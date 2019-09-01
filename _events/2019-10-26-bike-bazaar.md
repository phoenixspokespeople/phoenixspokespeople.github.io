---
title: "Fifth annual Bike Bazaar"
published: true
excerpt: "a special day of bicycle wares and bike goodness"
skip-title: true
facebook-event: 357731008267051
image:
  teaser: phoenix-public-market-open-air-market.png
  feature: bike-bazaar-banner.jpg
---

**Saturday, October 26**, **8 AM - 1 PM** at [Downtown Phoenix Public Market](http://phxpublicmarket.com/openair/).

Find your bike bliss at the fifth annual Bike Bazaar at the Phoenix Public Market. Like last year, in addition to bike-related clothes, art, jewelry and equipment there will be a bike swap!

Bike Bazaar vendors will be located along Pierce Street.

Registration for vendors is only $5 to Phoenix Spokes People, and 10% of sales at the end of the day for Phoenix Public Market. [Register as a vendor here!](http://psp.bike/bazaarvendor).

Free Admission and a raffle!

To pay vendor registration by card, use this button:

<!-- Load Stripe.js on your website. -->
<script src="https://js.stripe.com/v3"></script>

<button
  style="background-color:#6772E5;color:#FFF;padding:8px 12px;border:0;border-radius:4px;font-size:1em"
  id="checkout-button-sku_Fj9WX2BHPo3ke6"
  role="link"
>
  Checkout
</button>

<div id="error-message"></div>

<script>
  var stripe = Stripe('pk_live_JBEXFzc4NWuIO4UvZkltL0Dg');

  var checkoutButton = document.getElementById('checkout-button-sku_Fj9WX2BHPo3ke6');
  checkoutButton.addEventListener('click', function () {
    // When the customer clicks on the button, redirect
    // them to Checkout.
    stripe.redirectToCheckout({
      items: [{sku: 'sku_Fj9WX2BHPo3ke6', quantity: 1}],

      // Do not rely on the redirect to the successUrl for fulfilling
      // purchases, customers may not always reach the success_url after
      // a successful payment.
      // Instead use one of the strategies described in
      // https://stripe.com/docs/payments/checkout/fulfillment
      successUrl: 'http://www.phoenixspokespeople.org/events/2019-10-26-bike-bazaar/',
      cancelUrl: 'http://www.phoenixspokespeople.org/events/2019-10-26-bike-bazaar/',
    })
    .then(function (result) {
      if (result.error) {
        // If `redirectToCheckout` fails due to a browser or network
        // error, display the localized error message to your customer.
        var displayError = document.getElementById('error-message');
        displayError.textContent = result.error.message;
      }
    });
  });
</script>
