# Getting Started
## Installation
``` yarn add @stripe/react-stripe-js @stripe/stripe-js```

## Implementation
``` javascript 
import {loadStripe} from '@stripe/stripe-js'
import {
    Element,
    CardElement,
    useStripe,   "useStripe hook
    useElements  "useElements hook
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


