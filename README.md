# Redux-Form Storybook

A simple package to help you use redux-form components in your storybook stories.

### Install

With npm:
```
npm install --save-dev redux-form-storybook
```

With yarn:
```
yarn add --dev redux-form-storybook
```

### Use

import the `withReduxForm` component provided by the library and provide it to the `addDecorator` function. Simple as that!

```js
import React from 'react';
import { storiesOf } from '@storybook/react';
import { Field } from 'redux-form';
import withReduxForm from 'redux-form-storybook';

storiesOf('Field', module)
  .addDecorator(withReduxForm)
  .add('with text', () => (
      <Field
        name="onlyField"
        component="input"
        type="text"
      />
  ));

```
