# @react.app/components/Buttons

![MIT license](https://badgen.now.sh/badge/license/MIT)

[Source](https://github.com/xizon/uix-create-react-app/tree/main/src/components/Buttons)


## Examples

```js
import React from 'react';
import Button from '@react.app/components/Buttons';

let spreadOperator = {
  bgColor: 'info',
  btnName: 'Spread Operator',
};


export default () => {
  return (
    <>
		<Button bgColor='' btnName=''/>
		<Button bgColor='success' btnName='success'/>
		<Button bgColor='info' btnName='info'/>
		<Button bgColor='danger' btnName='danger'/>
		<Button bgColor='warning' btnName='warning'/>
		<Button {...spreadOperator}/>
    </>
  );
}

```