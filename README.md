<!<!DOCTYPE HTML>
<html>
    <head>
        <title>
            بوابت دفع
        </title>
    </head>
    <body>
<div id="paypal-button-container-P-31X48430D9126223XMWOVAAQ"></div>
<script src="https://www.paypal.com/sdk/js?client-id=AVclpd2g2BrIRs7KKO11m3ofn7__m4jcmPp52wfXtN9tK2ugNGO7-aBycjqnAievTL5zmzM6H6p3bpy3&vault=true&intent=subscription" data-sdk-integration-source="button-factory"></script>
<script>
  paypal.Buttons({
      style: {
          shape: 'pill',
          color: 'gold',
          layout: 'vertical',
          label: 'paypal'
      },
      createSubscription: function(data, actions) {
        return actions.subscription.create({
          /* Creates the subscription */
          plan_id: 'P-31X48430D9126223XMWOVAAQ'
        });
      },
      onApprove: function(data, actions) {
        alert(data.subscriptionID); // You can add optional success message for the subscriber here
      }
  }).render('#paypal-button-container-P-31X48430D9126223XMWOVAAQ'); // Renders the PayPal button
</script>
    </body>
</html>
