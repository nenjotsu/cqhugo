---
title: Pricing
toc: false
width: full
---

<div id="paypal-button-container-P-3Y797500VW949051NNCAZYQY"></div>
<script src="https://www.paypal.com/sdk/js?client-id=AU3eC8QiWaigvc5IPxQbJIOmmHW901BwSUtrkBAr2u5eMujcPV4hbJiukX_EvMwq5g8wRnQAyLPElb-E&vault=true&intent=subscription" data-sdk-integration-source="button-factory"></script>
<script>
  paypal.Buttons({
      style: {
          shape: 'rect',
          color: 'blue',
          layout: 'horizontal',
          label: 'subscribe'
      },
      createSubscription: function(data, actions) {
        return actions.subscription.create({
          /* Creates the subscription */
          plan_id: 'P-3Y797500VW949051NNCAZYQY'
        });
      },
      onApprove: function(data, actions) {
        alert(data.subscriptionID); // You can add optional success message for the subscriber here
      }
  }).render('#paypal-button-container-P-3Y797500VW949051NNCAZYQY'); // Renders the PayPal button
</script>
{{< cards >}}
  {{< card link="/" title="Classical $49.99/mo" image="fractal-hassan-XoNj0ulsn1Y-unsplash.jpg" subtitle="Basic" >}}
  {{< card link="/" title="Quantum $79.99/mo" image="karlis-reimanis-Y31Z6Mf7rys-unsplash.jpg" subtitle="Essential" >}}
  {{< card link="/" title="Superposition $199.99/mo" image="dynamic-wang-vNCBkSX3Nbo-unsplash.jpg" subtitle="Pro" >}}
{{< /cards >}}

| **Plan**   | Currency Pairs     | Gold   | HIN | Support | API Access | Webhook | Custom Strategy | Reports | Analytics | 
| --------  | -------- | ------ |--------  | -------- | ------ |--------  | -------- | ------ |--------  |
| **Classical** | ✅  |  |  |  |  |  || ✅  | ✅  |
| **Quantum** | ✅  | ✅  |  | ✅  |  ||  | ✅  | ✅  |
| **Superposition** | ✅ | ✅ |✅ | ✅ |✅ | ✅ |✅ | ✅ |✅ | ✅ |