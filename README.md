### Install

```
npm install --save-dev redux-form-storybook
```

```
yarn add --dev redux-form-storybook
```

### Use

```
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
