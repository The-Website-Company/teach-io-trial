# Teach IO Fullstack Trial Task

Create a payment tracking app that **stores** payments to a given Stripe account with the ability to **refund** a payment from the app.

Use the following tech stack:
* Node.js
* MongoDB (using Mongoose)
* React (using functional components and hooks)

You will need to integrate with Stripe using its API and Webhooks.

You should spend no longer than **4 hours** completing this task. If you are unable to finish the task, please let us know:
* What were the main blockers?
* What would your next steps would be if you had more time?

Please include a README with setup instructions to get the app up and running with _any_ Stripe account.

## Acceptance Criteria
* A list of payments is displayed to a user and should include the:
  * Stripe customer ID
  * Payment amount and currency
  * Date of payment
* Each payment should have the option to **refund**. Payments that have already been refunded should be marked as such.
* Incoming payments to the Stripe account should be stored in the database.

## Assumptions
* Payments will be created manually in [Stripe dashboard](https://dashboard.stripe.com/test/payments/new).
* Payments will have a customer, i.e. the "Customer" field will not be left blank when creating the payment in Stripe.
* Payments will be one-off _not_ subscriptions.

## Helpful Resources/Hints
You will need to integrate with Stripe using its API and Webhooks.
If you're not familiar with Stripe, these docs are a good place to start:
  * [Webhooks](https://stripe.com/docs/webhooks)
  * [PaymentIntents lifecycle](https://stripe.com/docs/payments/intents#intent-statuses)
  * [Server-side libraries](https://stripe.com/docs/libraries#server-side-libraries)
  * [Create a refund](https://stripe.com/docs/api/refunds/create)

Since webhooks need to be publicly accessible, you might need to use something like [ngrok](https://ngrok.com/).
