# Getting Started
## Installation
``` yarn add @stripe/react-stripe-js @stripe/stripe-js```

## Implementation
## At App.js
```javascript
import CheckoutForm from './CheckoutForm';
import {loadStripe} from '@stripe/stripe-js';  
import {Element} from '@stripe/react-stripe-js';
const App = ({}) => {

return(
//load stripe passing a public test key
 const stripePromise = loadStripe('pk_test_51HOL0GJ070ZzR858iGm2v2O5CQuZKgmL6BkY1O7V1Zr32QRMA5S55kDJbv0DKBCBj57UW0cYlT16KuOUIMQOQc8t00sT61i6gv');
 return(
<Element stripe={stripePromise}>
<CheckoutForm/>
</Element>
)
}
export default App
```
``` javascript 
import {
    Element,
    CardElement,
    useStripe,   "useStripe hook
    useElements  "useElements hook
   } from '@stripe/react-stripe-js'
cosnt CheckoutForm = () => {
const stripePromise = loadStripe('publish_key');
return(
<Elements stripe={stripePromise}>
<form>
<CardElement/>
</form>
</Elements>
)
}
```


