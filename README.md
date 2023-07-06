# Request Response Cycle, APIs, and Postman Lab

You will be working with a free API of your choice for this lab.

## Getting Started

1. Choose an API that has no auth and no CORS from the following list: [public APIs](https://github.com/public-apis/public-apis)
1. Write your answers in this README.md file. Do not delete the questions. Write your answers after the `>`. If you need to write more than one paragraph, add more `>`.

## Instructions

Do your best to answer the questions with specific details when required fully. Writing about code clearly and thoroughly is a critical skill to practice. 

- Which one did you choose? Provide the name and base URL

> I Chose the Razorpay API ; https://razorpay.com/docs/#home-payments

- What purpose is this API for (education/fun and games/information/etc.)?

> The purpose of this API is to give users a firctionless money mangment platfrom

- What is the URL of the documentation?

> https://razorpay.com/about/

- What is the full URL of one endpoint?

> https://razorpay.com/docs/payments/payment-gateway/ecommerce-plugins/

- What is a sample of the data from the endpoint (copy and paste results from Postman, ok to shorten if it’s over 100 lines)? Be sure to wrap your answer in the correct formatting for code/JSON.

```json
<!doctype html>
<script>
	window.BASE_NAME="/docs/"
</script>
<script>
	window.__NAVIGATION__ = [{"title":"Home","path":"/","iconName":"home","children":[]},{"title":"Get Started","path":"/get-started","iconName":"paper-plane","children":[]},{"title":"Payments","path":"/payments","iconName":"card","children":[{"title":"Razorpay Payments","path":"payments","children":[]},{"title":"Sign Up","path":"","children":[{"title":"Create a Razorpay Account","path":"payments/easy-create-account","children":[]},{"title":"Submit KYC Details","path":"payments/easy-submit-kyc","children":[]},{"title":"Business Types and KYC Documents","path":"payments/business-types-kyc-documents","children":[]},{"title":"Account Activation Support","path":"payments/account-activation-support","children":[]},{"title":"Frequently Asked Questions (FAQs)","path":"payments/faqs","children":[]}],"layout":""},{"title":"Dashboard","path":"","children":[{"title":"About Razorpay Dashboard","path":"payments/dashboard","children":[]},{"title":"Home Page","path":"payments/dashboard/home","children":[]},{"title":"Test and Live Modes","path":"payments/dashboard/test-live-modes","children":[]},{"title":"Reports","path":"payments/dashboard/reports","children":[]},{"title":"Account & Settings","path":"","children":[{"title":"About Account & Settings","path":"payments/dashboard/account-settings","children":[]},{"title":"Profile","path":"payments/dashboard/account-settings/profile","children":[]},{"title":"Credits","path":"payments/dashboard/account-settings/credits","children":[]},{"title":"Balances","path":"payments/dashboard/account-settings/balances","children":[]},{"title":"Razorpay Trusted Business Badge","path":"payments/dashboard/account-settings/trusted-badge","children":[]},{"title":"Manage Team","path":"payments/dashboard/account-settings/manage-team","children":[]},{"title":"Your Support Tickets","path":"payments/dashboard/account-settings/support-tickets","children":[]},{"title":"Configuration","path":"payments/dashboard/account-settings/configuration","children":[]},{"title":"API Keys","path":"payments/dashboard/account-settings/api-keys","children":[]},{"title":"Payment Methods","path":"payments/dashboard/account-settings/payment-methods","children":[]},{"title":"Reminders","path":"payments/dashboard/account-settings/reminders","children":[]}],"layout":""},{"title":"FAQs","path":"payments/dashboard/faqs","children":[]},{"title":"Contact Support","path":"payments/dashboard/support","children":[]}],"layout":""},{"title":"Customers","path":"","children":[{"title":"About Customers","path":"payments/customers","children":[]},{"title":"Customer Refunds","path":"payments/customers/customer-refunds","children":[]}],"layout":""},{"title":"Orders","path":"","children":[{"title":"About Orders","path":"payments/orders","children":[]},{"title":"Create Orders","path":"payments/orders/create","children":[]},{"title":"Dashboard","path":"payments/orders/dashboard","children":[]},{"title":"Orders APIs","path":"payments/orders/apis","children":[]}],"layout":""},{"title":"Payments","path":"","children":[{"title":"About Payments","path":"payments/payments","children":[]},{"title":"Test Card Details","path":"payments/payments/test-card-details","children":[]},{"title":"Test UPI ID Details","path":"payments/payments/test-upi-details","children":[]},{"title":"Payment Capture Settings","path":"payments/payments/capture-settings","children":[]},{"title":"International Payments","path":"","children":[{"title":"About International Payment Support","path":"payments/payments/international-payments","children":[]},{"title":"Address Verification System","path":"payments/payments/address-verification-system","children":[]},{"title":"Accept International Payments via Local Currency Bank Accounts","path":"payments/payments/accept-international-payments-via-local-currency-bank-accounts","children":[]},{"title":"Accept International Payments via SWIFT Transfer","path":"payments/payments/accept-international-payments-via-swift-transfer","children":[]},{"title":"International Business Accepting Payments From Indian Customers","path":"payments/payments/accept-international-payments-from-india","children":[]}],"layout":""},{"title":"Manage Late Authorised Payments","path":"","children":[{"title":"Late Payment Authorisations","path":"payments/payments/late-authorisation","children":[]},{"title":"Handle Late Authorised Payments","path":"payments/payments/late-authorisation/handle","children":[]}],"layout":""},{"title":"Dashboard","path":"payments/payments/dashboard","children":[]},{"title":"Payments APIs","path":"payments/payments/apis","children":[]},{"title":"Success Rate Analytics","path":"payments/payments/success-rate-analytics","children":[]},{"title":"Downtimes Updates","path":"payments/payments/downtime-updates","children":[]},{"title":"FAQs","path":"payments/payments/faqs","children":[]}],"layout":""},{"title":"Payment Methods","path":"","children":[{"title":"About Payment Methods","path":"payments/payment-methods","children":[]},{"title":"Bank Transfer","path":"payments/payment-methods/bank-transfer","children":[]},{"title":"Cards","path":"","children":[{"title":"About Card Payments","path":"payments/payment-methods/cards","children":[]},{"title":"Features","path":"","children":[{"title":"3D Secure 2.0 Authentication Protocol (3DS2)","path":"payments/payment-methods/cards/features/3ds2.0","children":[]},{"title":"Save Customer Card Details at Standard Checkout","path":"payments/payment-methods/cards/features/saved-cards","children":[]},{"title":"Manage Saved Cards","path":"payments/payment-methods/cards/features/manage","children":[]},{"title":"CVV-less Flow for Card Payments","path":"payments/payment-methods/cards/features/cvv-less-flow","children":[]}],"layout":""}],"layout":""},{"title":"EMI","path":"","children":[{"title":"About EMI","path":"payments/payment-methods/emi","children":[]},{"title":"Debit Card EMI","path":"payments/payment-methods/emi/debit-card-emi","children":[]},{"title":"Credit Card EMI","path":"","children":[{"title":"About Credit Card EMIs - Standard Checkout","path":"payments/payment-methods/emi/credit-card-emi","children":[]},{"title":"OneCard","path":"payments/payment-methods/emi/credit-card-emi/onecard","children":[]}],"layout":""},{"title":"Cardless EMI","path":"","children":[{"title":"About Cardless EMI - Standard Checkout","path":"payments/payment-methods/emi/cardless-emi","children":[]},{"title":"axio","path":"","children":[{"title":"About axio Cardless EMI","path":"payments/payment-methods/emi/cardless-emi/axio","children":[]},{"title":"Display axio on Standard Checkout","path":"payments/payment-methods/emi/cardless-emi/axio/checkout-configuration","children":[]},{"title":"FAQs","path":"payments/payment-methods/emi/cardless-emi/axio/faqs","children":[]}],"layout":""}],"layout":""},{"title":"No Cost EMI","path":"","children":[{"title":"About No Cost EMI","path":"payments/payment-methods/emi/no-cost-emi","children":[]},{"title":"Bajaj Finserv","path":"payments/payment-methods/emi/no-cost-emi/bajaj-finserv","children":[]}],"layout":""},{"title":"Frequently Asked Questions (FAQs)","path":"payments/payment-methods/emi/faqs","children":[]}],"layout":""},{"title":"Instant International Bank Transfer","path":"payments/payment-methods/instant-international-bank-transfer","children":[]},{"title":"MOTO","path":"","children":[{"title":"About MOTO Payments","path":"payments/payment-methods/moto","children":[]},{"title":"MOTO Batch Card Payments","path":"payments/payment-methods/moto/batch","children":[]}],"layout":""},{"title":"Netbanking","path":"payments/payment-methods/netbanking","children":[]},{"title":"Pay Later","path":"payments/payment-methods/pay-later","children":[]},{"title":"FPX","path":"payments/payment-methods/fpx","children":[]},{"title":"UPI","path":"","children":[{"title":"About UPI","path":"payments/payment-methods/upi","children":[]},{"title":"UPI Intent","path":"","children":[{"title":"About UPI Intent","path":"payments/payment-methods/upi/upi-intent","children":[]},{"title":"Android","path":"payments/payment-methods/upi/upi-intent/android","children":[]},{"title":"iOS","path":"payments/payment-methods/upi/upi-intent/ios","children":[]},{"title":"Mobile Web","path":"payments/payment-methods/upi/upi-intent/mobile-web","children":[]}],"layout":""},{"title":"Google Pay","path":"","children":[{"title":"About Google Pay","path":"payments/payment-methods/upi/google-pay","children":[]},{"title":"Standard Checkout","path":"payments/payment-methods/upi/google-pay/standard-integration","children":[]}],"layout":""},{"title":"Omnichannel Checkout","path":"","children":[{"title":"About Google Pay Omnichannel Checkout","path":"payments/payment-methods/upi/google-pay/omnichannel","children":[]},{"title":"Standard Checkout","path":"payments/payment-methods/upi/google-pay/omnichannel/standard-integration","children":[]}],"layout":""},{"title":"Features","path":"","children":[{"title":"Saved VPA","path":"payments/payment-methods/upi/saved-vpa","children":[]},{"title":"Virtual Payment Address (VPA) Validation","path":"payments/payment-methods/upi/vpa-validation","children":[]},{"title":"RuPay Credit Card on UPI","path":"payments/payment-methods/upi/cc-on-upi","children":[]}],"layout":""},{"title":"List of Supported UPI Apps","path":"payments/payment-methods/upi/supported-apps","children":[]},{"title":"Turbo UPI","path":"payments/payment-methods/upi/turbo-upi","children":[]}],"layout":""},{"title":"Wallets","path":"","children":[{"title":"Amazon Pay","path":"payments/payment-methods/wallets/amazon-pay","children":[]},{"title":"PayPal","path":"payments/payment-methods/wallets/paypal","children":[]},{"title":"Bajaj Pay","path":"payments/payment-methods/wallets/bajaj-pay","children":[]},{"title":"Touch'n Go","path":"payments/payment-methods/wallets/touch-n-go","children":[]},{"title":"GrabPay","path":"payments/payment-methods/wallets/grab-pay","children":[]}],"layout":""},{"title":"Transaction Limits","path":"","children":[{"title":"Transaction Limits for Payment Methods","path":"payments/payment-methods/transaction-limits","children":[]},{"title":"UPI Transaction Limits","path":"payments/payment-methods/transaction-limits/upi","children":[]}],"layout":""}],"layout":""},{"title":"Settlements","path":"","children":[{"title":"About Settlements","path":"payments/settlements","children":[]},{"title":"Dashboard","path":"payments/settlements/dashboard","children":[]},{"title":"Instant Settlements","path":"payments/settlements/instant","children":[]},{"title":"Settlements APIs","path":"payments/settlements/apis","children":[]},{"title":"FAQs","path":"payments/settlements/faqs","children":[]}],"layout":""},{"title":"Refunds","path":"","children":[{"title":"About Refunds","path":"payments/refunds","children":[]},{"title":"Normal Refunds","path":"payments/refunds/normal","children":[]},{"title":"Instant Refunds","path":"","children":[{"title":"About Instant Refunds","path":"payments/refunds/instant","children":[]},{"title":"Supported Payment Methods","path":"payments/refunds/supported-payment-methods","children":[]}],"layout":""},{"title":"Batch Refunds","path":"payments/refunds/batch","children":[]},{"title":"EMI and Pay Later Refunds","path":"payments/refunds/emi-pay-later","children":[]},{"title":"Dashboard","path":"","children":[{"title":"Issue Refunds","path":"payments/refunds/issue","children":[]},{"title":"View Refunds","path":"payments/refunds/view","children":[]},{"title":"Set Refund Speed","path":"payments/refunds/refund-speed","children":[]}],"layout":""},{"title":"Handle Refund Errors","path":"payments/refunds/errors","children":[]},{"title":"Refunds APIs","path":"payments/refunds/apis","children":[]},{"title":"Subscribe to Webhooks","path":"payments/refunds/subscribe-to-webhooks","children":[]},{"title":"Refund Communication","path":"payments/refunds/communication","children":[]},{"title":"FAQs","path":"payments/refunds/faqs","children":[]}],"layout":""},{"title":"Disputes","path":"","children":[{"title":"About Disputes","path":"payments/disputes","children":[]},{"title":"Submit Evidence","path":"payments/disputes/submit-evidence","children":[]},{"title":"Dashboard","path":"payments/disputes/dashboard","children":[]},{"title":"Disputes APIs","path":"payments/disputes/apis","children":[]},{"title":"FAQs","path":"payments/disputes/faqs","children":[]}],"layout":""},{"title":"Payment Gateway","path":"","children":[{"title":"About Payment Gateway","path":"payments/payment-gateway","children":[]},{"title":"Features","path":"payments/payment-gateway/features","children":[]},{"title":"Get Started","path":"payments/payment-gateway/get-started","children":[]},{"title":"How Payment Gateway Works","path":"payments/payment-gateway/how-it-works","children":[]},{"title":"Web Integrations","path":"","children":[{"title":"About Standard Web Checkout Integration","path":"payments/payment-gateway/web-integration/standard","children":[]},{"title":"1. Build Integration","path":"payments/payment-gateway/web-integration/standard/build-integration","children":[]},{"title":"2. Test Integration","path":"payments/payment-gateway/web-integration/standard/test-integration","children":[]},{"title":"3. Go-live Checklist","path":"payments/payment-gateway/web-integration/standard/go-live-checklist","children":[]},{"title":"Configure Payment Methods","path":"","children":[{"title":"About Payment Methods Configuration","path":"payments/payment-gateway/web-integration/standard/configure-payment-methods","children":[]},{"title":"Understand the Configuration","path":"payments/payment-gateway/web-integration/standard/configure-payment-methods/understand-configuration","children":[]},{"title":"Display the Configuration","path":"payments/payment-gateway/web-integration/standard/configure-payment-methods/display-configuration","children":[]},{"title":"Sample Codes","path":"payments/payment-gateway/web-integration/standard/configure-payment-methods/sample-code","children":[]},{"title":"Supported Methods","path":"payments/payment-gateway/web-integration/standard/configure-payment-methods/supported-methods","children":[]}],"layout":""},{"title":"Best Practices","path":"payments/payment-gateway/web-integration/standard/best-practices","children":[]},{"title":"Troubleshooting & FAQs","path":"payments/payment-gateway/web-integration/standard/troubleshooting-faqs","children":[]},{"title":"WebView for Mobile Apps","path":"","children":[{"title":"About Webview for Mobile Apps","path":"payments/payment-gateway/web-integration/standard/webview","children":[]},{"title":"UPI Intent","path":"","children":[{"title":"Android","path":"payments/payment-gateway/web-integration/standard/webview/upi-intent-android","children":[]},{"title":"iOS","path":"payments/payment-gateway/web-integration/standard/webview/upi-intent-ios","children":[]}],"layout":""}],"layout":""}],"layout":""},{"title":"Hosted Checkout","path":"","children":[{"title":"Integrate with Hosted Checkout","path":"payments/payment-gateway/web-integration/hosted","children":[]},{"title":"1. Build Integration","path":"payments/payment-gateway/web-integration/hosted/build-integration","children":[]},{"title":"2. Test Integration","path":"payments/payment-gateway/web-integration/hosted/test-integration","children":[]},{"title":"3. Go-live Checklist","path":"payments/payment-gateway/web-integration/hosted/go-live-checklist","children":[]},{"title":"Best Practices for Hosted Checkout Integration","path":"payments/payment-gateway/web-integration/hosted/best-practices","children":[]}],"layout":""},{"title":"Android Integration","path":"","children":[{"title":"Integrate With Android Standard SDK","path":"payments/payment-gateway/android-integration/standard","children":[]},{"title":"1. Build Integration","path":"payments/payment-gateway/android-integration/standard/build-integration","children":[]},{"title":"2. Test Integration","path":"payments/payment-gateway/android-integration/standard/test-integration","children":[]},{"title":"3. Go-live Checklist","path":"payments/payment-gateway/android-integration/standard/go-live-checklist","children":[]},{"title":"Additional Support for Payment Methods","path":"payments/payment-gateway/android-integration/standard/payment-methods","children":[]},{"title":"Customisation Options","path":"payments/payment-gateway/android-integration/standard/customisation","children":[]},{"title":"Override Minimum SDK Version","path":"payments/payment-gateway/android-integration/standard/override-minimum-sdk","children":[]},{"title":"Troubleshooting & FAQs","path":"payments/payment-gateway/android-integration/standard/troubleshooting-faqs","children":[]},{"title":"Google Play Console - Data Safety","path":"payments/payment-gateway/android-integration/standard/google-data-safety","children":[]}],"layout":""},{"title":"iOS Integration","path":"","children":[{"title":"Integrate with iOS Standard SDK","path":"payments/payment-gateway/ios-integration/standard","children":[]},{"title":"1. Build Integration","path":"payments/payment-gateway/ios-integration/standard/build-integration","children":[]},{"title":"2. Test Integration","path":"payments/payment-gateway/ios-integration/standard/test-integration","children":[]},{"title":"3. Go-live Checklist","path":"payments/payment-gateway/ios-integration/standard/go-live-checklist","children":[]},{"title":"Troubleshooting & FAQs","path":"payments/payment-gateway/ios-integration/standard/troubleshooting-faqs","children":[]},{"title":"WebView for Mobile Apps","path":"payments/payment-gateway/ios-integration/webapp","children":[]}],"layout":""},{"title":"React Native","path":"","children":[{"title":"Integrate With React Native Standard SDK","path":"payments/payment-gateway/react-native-integration/standard","children":[]},{"title":"1. Build Integration (Android)","path":"payments/payment-gateway/react-native-integration/standard/build-integration-android","children":[]},{"title":"1. Build Integration (iOS)","path":"payments/payment-gateway/react-native-integration/standard/build-integration-ios","children":[]},{"title":"2. Test Integration","path":"payments/payment-gateway/react-native-integration/standard/test-integration","children":[]},{"title":"3. Go-live Checklist","path":"payments/payment-gateway/react-native-integration/standard/go-live-checklist","children":[]},{"title":"Troubleshooting & FAQs","path":"payments/payment-gateway/react-native-integration/standard/troubleshooting-faqs","children":[]}],"layout":""},{"title":"Cordova & Ionic","path":"","children":[{"title":"Integrate With Cordova Standard SDK","path":"payments/payment-gateway/cordova-integration","children":[]},{"title":"1. Build Integration","path":"payments/payment-gateway/cordova-integration/build-integration","children":[]},{"title":"2. Test Integration","path":"payments/payment-gateway/cordova-integration/test-integration","children":[]},{"title":"3. Go-live Checklist","path":"payments/payment-gateway/cordova-integration/go-live-checklist","children":[]},{"title":"Troubleshooting & FAQs","path":"payments/payment-gateway/cordova-integration/troubleshooting-faqs","children":[]}],"layout":""},{"title":"Flutter Plugin","path":"","children":[{"title":"Integrate with Flutter Standard SDK","path":"payments/payment-gateway/flutter-integration/standard","children":[]},{"title":"1. Build Integration","path":"payments/payment-gateway/flutter-integration/standard/build-integration","children":[]},{"title":"2. Test Integration","path":"payments/payment-gateway/flutter-integration/standard/test-integration","children":[]},{"title":"3. Go-live Checklist","path":"payments/payment-gateway/flutter-integration/standard/go-live-checklist","children":[]},{"title":"API Classes and Methods","path":"payments/payment-gateway/flutter-integration/standard/api","children":[]},{"title":"Troubleshooting & FAQs","path":"payments/payment-gateway/flutter-integration/standard/troubleshooting-faqs","children":[]}],"layout":""},{"title":"Capacitor Integration","path":"","children":[{"title":"Integrate With Capacitor Standard SDK","path":"payments/payment-gateway/capacitor-integration","children":[]},{"title":"1. Build Integration","path":"payments/payment-gateway/capacitor-integration/build-integration","children":[]},{"title":"2. Test Integration","path":"payments/payment-gateway/capacitor-integration/test-integration","children":[]},{"title":"3. Go-live Checklist","path":"payments/payment-gateway/capacitor-integration/go-live-checklist","children":[]},{"title":"Troubleshooting & FAQs","path":"payments/payment-gateway/capacitor-integration/troubleshooting-faqs","children":[]}],"layout":""},{"title":"Quick Integration","path":"","children":[{"title":"Integrate With Quick Checkout","path":"payments/payment-gateway/quick-integration","children":[]},{"title":"1. Build Integration","path":"payments/payment-gateway/quick-integration/build-integration","children":[]},{"title":"2. Test Integration","path":"payments/payment-gateway/quick-integration/test-integration","children":[]},{"title":"3. Go-live Checklist","path":"payments/payment-gateway/quick-integration/go-live-checklist","children":[]}],"layout":""},{"title":"Server Integration","path":"","children":[{"title":"About Server Integrations","path":"payments/server-integration","children":[]},{"title":".NET","path":"","children":[{"title":"Install Razorpay .NET SDK","path":"payments/server-integration/dot-net/install","children":[]},{"title":"Payment Gateway","path":"","children":[{"title":"Integrate With .NET SDK","path":"payments/server-integration/dot-net/payment-gateway","children":[]},{"title":"1. Build Integration","path":"payments/server-integration/dot-net/payment-gateway/build-integration","children":[]},{"title":"2. Test Integration","path":"payments/server-integration/dot-net/payment-gateway/test-integration","children":[]},{"title":"3. Go-live Checklist","path":"payments/server-integration/dot-net/payment-gateway/go-live-checklist","children":[]}],"layout":""},{"title":"Troubleshooting & FAQs","path":"payments/server-integration/dot-net/troubleshooting-faqs","children":[]}],"layout":""},{"title":"Go","path":"","children":[{"title":"Install Razorpay Go SDK","path":"payments/server-integration/go/install","children":[]},{"title":"Payment Gateway","path":"","children":[{"title":"Integrate With Go SDK","path":"payments/server-integration/go/payment-gateway","children":[]},{"title":"1. Build Integration","path":"payments/server-integration/go/payment-gateway/build-integration","children":[]},{"title":"2. Test Integration","path":"payments/server-integration/go/payment-gateway/test-integration","children":[]},{"title":"3. Go-live Checklist","path":"payments/server-integration/go/payment-gateway/go-live-checklist","children":[]}],"layout":""}],"layout":""},{"title":"Java","path":"","children":[{"title":"Install Razorpay Java SDK","path":"payments/server-integration/java/install","children":[]},{"title":"Payment Gateway","path":"","children":[{"title":"Integrate With Java SDK","path":"payments/server-integration/java/payment-gateway","children":[]},{"title":"1. Build Integration","path":"payments/server-integration/java/payment-gateway/build-integration","children":[]},{"title":"2. Test Integration","path":"payments/server-integration/java/payment-gateway/test-integration","children":[]},{"title":"3. Go-live Checklist","path":"payments/server-integration/java/payment-gateway/go-live-checklist","children":[]}],"layout":""},{"title":"Integrate with Other Razorpay Products","path":"payments/server-integration/java/others-integration","children":[]}],"layout":""},{"title":"Node.js","path":"","children":[{"title":"Install Razorpay Node.js SDK","path":"payments/server-integration/nodejs/install","children":[]},{"title":"Payment Gateway","path":"","children":[{"title":"Integrate With Node.js SDK","path":"payments/server-integration/nodejs/payment-gateway","children":[]},{"title":"1. Build Integration","path":"payments/server-integration/nodejs/payment-gateway/build-integration","children":[]},{"title":"2. Test Integration","path":"payments/server-integration/nodejs/payment-gateway/test-integration","children":[]},{"title":"3. Go-live Checklist","path":"payments/server-integration/nodejs/payment-gateway/go-live-checklist","children":[]}],"layout":""},{"title":"Integrate with Other Razorpay Products","path":"payments/server-integration/nodejs/others-integration","children":[]},{"title":"FAQs","path":"payments/server-integration/nodejs/faqs","children":[]}],"layout":""},{"title":"PHP","path":"","children":[{"title":"Install Razorpay PHP SDK","path":"payments/server-integration/php/install","children":[]},{"title":"Payment Gateway","path":"","children":[{"title":"Integrate With PHP SDK","path":"payments/server-integration/php/payment-gateway","children":[]},{"title":"1. Build Integration","path":"payments/server-integration/php/payment-gateway/build-integration","children":[]},{"title":"2. Test Integration","path":"payments/server-integration/php/payment-gateway/test-integration","children":[]},{"title":"3. Go-live Checklist","path":"payments/server-integration/php/payment-gateway/go-live-checklist","children":[]}],"layout":""},{"title":"Integrate with Other Razorpay Products","path":"payments/server-integration/php/others-integration","children":[]}],"layout":""},{"title":"Python","path":"","children":[{"title":"Install Razorpay Python SDK","path":"payments/server-integration/python/install","children":[]},{"title":"Payment Gateway","path":"","children":[{"title":"Integrate With Python SDK","path":"payments/server-integration/python/payment-gateway","children":[]},{"title":"1. Build Integration","path":"payments/server-integration/python/payment-gateway/build-integration","children":[]},{"title":"2. Test Integration","path":"payments/server-integration/python/payment-gateway/test-integration","children":[]},{"title":"3. Go-live Checklist","path":"payments/server-integration/python/payment-gateway/go-live-checklist","children":[]}],"layout":""},{"title":"Integrate with Other Razorpay Products","path":"payments/server-integration/python/others-integration","children":[]}],"layout":""},{"title":"Ruby","path":"","children":[{"title":"Install Razorpay Ruby SDK","path":"payments/server-integration/ruby/install","children":[]},{"title":"Payment Gateway","path":"","children":[{"title":"Integrate With Ruby SDK","path":"payments/server-integration/ruby/payment-gateway","children":[]},{"title":"1. Build Integration","path":"payments/server-integration/ruby/payment-gateway/build-integration","children":[]},{"title":"2. Test Integration","path":"payments/server-integration/ruby/payment-gateway/test-integration","children":[]},{"title":"3. Go-live Checklist","path":"payments/server-integration/ruby/payment-gateway/go-live-checklist","children":[]}],"layout":""}],"layout":""}],"layout":""}],"layout":""},{"title":"Ecommerce Plugins","path":"","children":[{"title":"About Ecommerce Plugins","path":"payments/payment-gateway/ecommerce-plugins","children":[]},{"title":"Arastta","path":"","children":[{"title":"Integrate With Arastta Plugin","path":"payments/payment-gateway/ecommerce-plugins/arastta","children":[]},{"title":"1. Build Integration","path":"payments/payment-gateway/ecommerce-plugins/arastta/build-integration","children":[]},{"title":"2. Test Integration","path":"payments/payment-gateway/ecommerce-plugins/arastta/test-integration","children":[]},{"title":"3. Go-live Checklist","path":"payments/payment-gateway/ecommerce-plugins/arastta/go-live-checklist","children":[]}],"layout":""},{"title":"Build Your Own","path":"","children":[{"title":"About Build Your Own Ecommerce Plugin","path":"payments/payment-gateway/ecommerce-plugins/build-your-own","children":[]},{"title":"Use Cases","path":"payments/payment-gateway/ecommerce-plugins/build-your-own/use-case","children":[]},{"title":"FAQs","path":"payments/payment-gateway/ecommerce-plugins/build-your-own/faqs","children":[]}],"layout":""},{"title":"BigCommerce","path":"","children":[{"title":"Integrate With BigCommerce Plugin","path":"payments/payment-gateway/ecommerce-plugins/bigcommerce","children":[]},{"title":"1. Build Integration","path":"payments/payment-gateway/ecommerce-plugins/bigcommerce/build-integration","children":[]},{"title":"2. Test Integration","path":"payments/payment-gateway/ecommerce-plugins/bigcommerce/test-integration","children":[]},{"title":"3. Go-live Checklist","path":"payments/payment-gateway/ecommerce-plugins/bigcommerce/go-live-checklist","children":[]},{"title":"Frequently Asked Questions (FAQs)","path":"payments/payment-gateway/ecommerce-plugins/bigcommerce/faqs","children":[]}],"layout":""},{"title":"Drupal Commerce","path":"","children":[{"title":"Integrate With Drupal Commerce Plugin","path":"payments/payment-gateway/ecommerce-plugins/drupal-commerce","children":[]},{"title":"1. Build Integration","path":"payments/payment-gateway/ecommerce-plugins/drupal-commerce/build-integration","children":[]},{"title":"2. Test Integration","path":"payments/payment-gateway/ecommerce-plugins/drupal-commerce/test-integration","children":[]},{"title":"3. Go-live Checklist","path":"payments/payment-gateway/ecommerce-plugins/drupal-commerce/go-live-checklist","children":[]},{"title":"Frequently Asked Questions (FAQs)","path":"payments/payment-gateway/ecommerce-plugins/drupal-commerce/troubleshooting-faqs","children":[]}],"layout":""},{"title":"Easy Digital Downloads","path":"","children":[{"title":"Integrate With Easy Digital Downloads Plugin","path":"payments/payment-gateway/ecommerce-plugins/easy-digital-downloads","children":[]},{"title":"1. Build Integration","path":"payments/payment-gateway/ecommerce-plugins/easy-digital-downloads/build-integration","children":[]},{"title":"2. Test Integration","path":"payments/payment-gateway/ecommerce-plugins/easy-digital-downloads/test-integration","children":[]},{"title":"3. Go-live Checklist","path":"payments/payment-gateway/ecommerce-plugins/easy-digital-downloads/go-live-checklist","children":[]}],"layout":""},{"title":"CS-Cart","path":"","children":[{"title":"Integrate with CS-Cart Plugin","path":"payments/payment-gateway/ecommerce-plugins/cs-cart","children":[]},{"title":"1. Build Integration","path":"payments/payment-gateway/ecommerce-plugins/cs-cart/build-integration","children":[]},{"title":"2. Test Integration","path":"payments/payment-gateway/ecommerce-plugins/cs-cart/test-integration","children":[]},{"title":"3. Go-live Checklist","path":"payments/payment-gateway/ecommerce-plugins/cs-cart/go-live-checklist","children":[]},{"title":"Troubleshooting & FAQs","path":"payments/payment-gateway/ecommerce-plugins/cs-cart/troubleshooting-faqs","children":[]}],"layout":""},{"title":"Gravity Forms","path":"","children":[{"title":"Integrate With Gravity Forms Plugin","path":"payments/payment-gateway/ecommerce-plugins/gravity-forms","children":[]},{"title":"1. Build Integration","path":"payments/payment-gateway/ecommerce-plugins/gravity-forms/build-integration","children":[]},{"title":"2. Test Integration","path":"payments/payment-gateway/ecommerce-plugins/gravity-forms/test-integration","children":[]},{"title":"3. Go-live Checklist","path":"payments/payment-gateway/ecommerce-plugins/gravity-forms/go-live-checklist","children":[]},{"title":"Troubleshooting & FAQs","path":"payments/payment-gateway/ecommerce-plugins/gravity-forms/troubleshooting-faqs","children":[]}],"layout":""},{"title":"Magento","path":"","children":[{"title":"Integrate with Magento Plugin","path":"payments/payment-gateway/ecommerce-plugins/magento","children":[]},{"title":"1. Build Integration","path":"payments/payment-gateway/ecommerce-plugins/magento/build-integration","children":[]},{"title":"2. Test Integration","path":"payments/payment-gateway/ecommerce-plugins/magento/test-integration","children":[]},{"title":"3. Go-live Checklist","path":"payments/payment-gateway/ecommerce-plugins/magento/go-live-checklist","children":[]},{"title":"Troubleshooting","path":"payments/payment-gateway/ecommerce-plugins/magento/troubleshooting","children":[]}],"layout":""},{"title":"OpenCart","path":"","children":[{"title":"Integrate With OpenCart Plugin","path":"payments/payment-gateway/ecommerce-plugins/open-cart","children":[]},{"title":"1. Build Integration","path":"payments/payment-gateway/ecommerce-plugins/open-cart/build-integration","children":[]},{"title":"2. Test Integration","path":"payments/payment-gateway/ecommerce-plugins/open-cart/test-integration","children":[]},{"title":"3. Go-live Checklist","path":"payments/payment-gateway/ecommerce-plugins/open-cart/go-live-checklist","children":[]},{"title":"Troubleshooting & FAQs","path":"payments/payment-gateway/ecommerce-plugins/open-cart/troubleshooting-faqs","children":[]}],"layout":""},{"title":"Prestashop","path":"","children":[{"title":"Integrate With Prestashop Plugin","path":"payments/payment-gateway/ecommerce-plugins/prestashop","children":[]},{"title":"1. Build Integration","path":"payments/payment-gateway/ecommerce-plugins/prestashop/build-integration","children":[]},{"title":"2. Test Integration","path":"payments/payment-gateway/ecommerce-plugins/prestashop/test-integration","children":[]},{"title":"3. Go Live Checklist","path":"payments/payment-gateway/ecommerce-plugins/prestashop/go-live-checklist","children":[]},{"title":"Troubleshooting & FAQs","path":"payments/payment-gateway/ecommerce-plugins/prestashop/troubleshooting-faqs","children":[]}],"layout":""},{"title":"Shopify - Razorpay Secure","path":"","children":[{"title":"Integrate With Shopify Plugin","path":"payments/payment-gateway/ecommerce-plugins/shopify","children":[]},{"title":"1. Build Integration","path":"payments/payment-gateway/ecommerce-plugins/shopify/build-integration","children":[]},{"title":"2. Go Live Checklist","path":"payments/payment-gateway/ecommerce-plugins/shopify/go-live","children":[]},{"title":"Migration Steps","path":"payments/payment-gateway/ecommerce-plugins/shopify/migration-steps","children":[]},{"title":"Accept International Payments","path":"payments/payment-gateway/ecommerce-plugins/shopify/international-payments","children":[]},{"title":"Reconcile Shopify Orders on Razorpay Dashboard","path":"payments/payment-gateway/ecommerce-plugins/shopify/reconcile-payments","children":[]},{"title":"Features","path":"","children":[{"title":"Display Offers on Checkout","path":"payments/payment-gateway/ecommerce-plugins/shopify/features/display-offers","children":[]},{"title":"Initiate Refunds","path":"payments/payment-gateway/ecommerce-plugins/shopify/features/initiate-refunds","children":[]}],"layout":""},{"title":"Frequently Asked Questions (FAQs)","path":"payments/payment-gateway/ecommerce-plugins/shopify/faqs","children":[]}],"layout":""},{"title":"WHMCS","path":"","children":[{"title":"Integrate With WHMCS Plugin","path":"payments/payment-gateway/ecommerce-plugins/whmcs","children":[]},{"title":"1. Build Integration","path":"payments/payment-gateway/ecommerce-plugins/whmcs/build-integration","children":[]},{"title":"2. Test Integration","path":"payments/payment-gateway/ecommerce-plugins/whmcs/test-integration","children":[]},{"title":"3. Go-live Checklist","path":"payments/payment-gateway/ecommerce-plugins/whmcs/go-live-checklist","children":[]},{"title":"Frequently Asked Questions (FAQs)","path":"payments/payment-gateway/ecommerce-plugins/whmcs/faqs","children":[]}],"layout":""},{"title":"Wix","path":"","children":[{"title":"Integrate with Wix Extension","path":"payments/payment-gateway/ecommerce-plugins/wix","children":[]},{"title":"1. Build Integration","path":"payments/payment-gateway/ecommerce-plugins/wix/build-integration","children":[]},{"title":"2. Test Integration","path":"payments/payment-gateway/ecommerce-plugins/wix/test-integration","children":[]},{"title":"3. Go-live Checklist","path":"payments/payment-gateway/ecommerce-plugins/wix/go-live-checklist","children":[]},{"title":"Frequently Asked Questions (FAQs)","path":"payments/payment-gateway/ecommerce-plugins/wix/faqs","children":[]}],"layout":""},{"title":"Woocommerce","path":"","children":[{"title":"Integrate With WooCommerce Plugin","path":"payments/payment-gateway/ecommerce-plugins/woocommerce","children":[]},{"title":"1. Build Integration","path":"payments/payment-gateway/ecommerce-plugins/woocommerce/build-integration","children":[]},{"title":"2. Test Integration","path":"payments/payment-gateway/ecommerce-plugins/woocommerce/test-integration","children":[]},{"title":"3. Go-live Checklist","path":"payments/payment-gateway/ecommerce-plugins/woocommerce/go-live-checklist","children":[]},{"title":"Troubleshooting & FAQs","path":"payments/payment-gateway/ecommerce-plugins/woocommerce/troubleshooting-faqs","children":[]}],"layout":""},{"title":"WordPress","path":"","children":[{"title":"Integrate With WordPress Plugin","path":"payments/payment-gateway/ecommerce-plugins/wordpress","children":[]},{"title":"1. Build Integration","path":"payments/payment-gateway/ecommerce-plugins/wordpress/build-integration","children":[]},{"title":"2. Test Integration","path":"payments/payment-gateway/ecommerce-plugins/wordpress/test-integration","children":[]},{"title":"3. Go Live Checklist","path":"payments/payment-gateway/ecommerce-plugins/wordpress/go-live-checklist","children":[]},{"title":"Frequently Asked Questions (FAQs)","path":"payments/payment-gateway/ecommerce-plugins/wordpress/faqs","children":[]}],"layout":""}],"layout":""},{"title":"Magic Checkout","path":"","children":[{"title":"About Magic Checkout","path":"payments/magic-checkout","children":[]},{"title":"Integrate Magic Checkout on Website","path":"payments/magic-checkout/web","children":[]},{"title":"Integrate Magic Checkout with WooCommerce Website","path":"","children":[{"title":"Integration Steps","path":"payments/magic-checkout/woocommerce","children":[]},{"title":"Configuration Options","path":"payments/magic-checkout/woocommerce/configuration","children":[]}],"layout":""},{"title":"Integrate Magic Checkout With Shopify Website","path":"payments/magic-checkout/shopify","children":[]},{"title":"Integrate with Logistics Partners","path":"","children":[{"title":"About Logistics Partners Integration","path":"payments/magic-checkout/logistics-partners","children":[]},{"title":"Shiprocket","path":"payments/magic-checkout/logistics-partners/shiprocket","children":[]},{"title":"Delhivery","path":"payments/magic-checkout/logistics-partners/delhivery","children":[]}],"layout":""},{"title":"Dashboard Actions","path":"","children":[{"title":"Settings","path":"payments/magic-checkout/settings","children":[]},{"title":"Upload Order Status","path":"","children":[{"title":"About Order Status Upload","path":"payments/magic-checkout/upload-order-status","children":[]},{"title":"Delivery Status","path":"payments/magic-checkout/upload-order-status/delivery-statuses","children":[]},{"title":"Order History","path":"payments/magic-checkout/upload-order-status/order-history","children":[]}],"layout":""},{"title":"Prepay COD","path":"payments/magic-checkout/prepay-cod","children":[]},{"title":"RTO Analytics","path":"","children":[{"title":"About RTO Analytics","path":"payments/magic-checkout/rto-analytics","children":[]},{"title":"Risk Report","path":"payments/magic-checkout/rto-analytics/risk-report","children":[]},{"title":"RTO Insights","path":"payments/magic-checkout/rto-analytics/rto-insights","children":[]}],"layout":""},{"title":"Manually Review COD Orders","path":"","children":[{"title":"About Manual Review of COD Orders","path":"payments/magic-checkout/review-cod-orders","children":[]},{"title":"COD Orders Review Workflow","path":"payments/magic-checkout/review-cod-orders/workflow","children":[]}],"layout":""}],"layout":""},{"title":"Troubleshooting & FAQs","path":"payments/magic-checkout/troubleshooting-faqs","children":[]}],"layout":""},{"title":"Payment Links","path":"","children":[{"title":"About Payment Links","path":"payments/payment-links","children":[]},{"title":"Payment Link Types","path":"","children":[{"title":"Standard Payment Links","path":"payments/payment-links/standard","children":[]},{"title":"UPI Payment Links (New)","path":"payments/payment-links/upi","children":[]}],"layout":""},{"title":"How Payment Link Works","path":"payments/payment-links/how-it-works","children":[]},{"title":"Payment Link States","path":"payments/payment-links/states","children":[]},{"title":"Dashboard","path":"","children":[{"title":"Create a Payment Link","path":"payments/payment-links/create","children":[]},{"title":"Enable Partial Payments","path":"payments/payment-links/partial-payments","children":[]},{"title":"Edit a Payment Link","path":"payments/payment-links/edit","children":[]},{"title":"Cancel a Payment Link","path":"payments/payment-links/cancel","children":[]},{"title":"Duplicate a Payment Link","path":"payments/payment-links/duplicate","children":[]},{"title":"Search a Payment Link","path":"payments/payment-links/search","children":[]},{"title":"Resend a Payment Link","path":"payments/payment-links/resend","children":[]},{"title":"Create Payment Links in Batches","path":"payments/payment-links/batch","children":[]},{"title":"Send Reminders","path":"payments/payment-links/reminders","children":[]}],"layout":""},{"title":"WhatsApp Bot for Payment Links","path":"payments/payment-links/whatsapp-bot","children":[]},{"title":"Advanced Options","path":"","children":[{"title":"Offers on Payment Links","path":"payments/payment-links/offers","children":[]},{"title":"Bank Transfers","path":"","children":[{"title":"Receive Payments via Bank Transfer","path":"payments/payment-links/bank-transfer","children":[]},{"title":"FAQs","path":"payments/payment-links/bank-transfer-faqs","children":[]}],"layout":""}],"layout":""},{"title":"Manage Team","path":"payments/payment-links/manage-team","children":[]},{"title":"View Reports","path":"payments/payment-links/view-reports","children":[]},{"title":"Payment Links APIs","path":"payments/payment-links/apis","children":[]},{"title":"Subscribe to Webhooks","path":"payments/payment-links/subscribe-to-webhooks","children":[]},{"title":"FAQs (Frequently Asked Questions)","path":"payments/payment-links/faqs","children":[]},{"title":"Glossary","path":"payments/payment-links/glossary","children":[]}],"layout":""},{"title":"Payment Button","path":"","children":[{"title":"About Payment Button","path":"payments/payment-button","children":[]},{"title":"How Payment Button Works","path":"payments/payment-button/how-it-works","children":[]},{"title":"Payment Button States","path":"payments/payment-button/states","children":[]},{"title":"Dashboard","path":"","children":[{"title":"Quick Pay Button","path":"payments/payment-button/quick-pay","children":[]},{"title":"Buy Now Button","path":"payments/payment-button/buy-now","children":[]},{"title":"Donations Button","path":"payments/payment-button/donations","children":[]},{"title":"Custom Button","path":"payments/payment-button/custom","children":[]},{"title":"Manage","path":"","children":[{"title":"Manage Payment Button","path":"payments/payment-button/manage","children":[]},{"title":"Prefill Amount Fields","path":"payments/payment-button/manage/prefill-amount-fields","children":[]}],"layout":""},{"title":"Search a Payment Button","path":"payments/payment-button/search","children":[]}],"layout":""},{"title":"Configure Payment Receipts","path":"","children":[{"title":"Configure Generic Payment Button Receipt","path":"payments/payment-button/receipt","children":[]},{"title":"Configure 80G-enabled Payment Button Receipt","path":"payments/payment-button/80g-receipt","children":[]}],"layout":""},{"title":"Plugins","path":"","children":[{"title":"About Plugins","path":"payments/payment-button/supported-platforms","children":[]},{"title":"WordPress","path":"","children":[{"title":"WordPress Payment Plugin","path":"payments/payment-button/supported-platforms/wordpress","children":[]},{"title":"WordPress Elementor Payment Plugin","path":"payments/payment-button/supported-platforms/wordpress/elementor","children":[]},{"title":"WordPress SiteOrigin Payment Plugin","path":"payments/payment-button/supported-platforms/wordpress/site-origin","children":[]},{"title":"WordPress Visual Composer Payment Plugin","path":"payments/payment-button/supported-platforms/wordpress/visual-composer","children":[]},{"title":"Create a WordPress Website","path":"payments/payment-button/supported-platforms/wordpress/create-website","children":[]}],"layout":""}],"layout":""},{"title":"Add Facebook Pixel on Payment Success Page","path":"payments/payment-button/add-fb-pixel","children":[]},{"title":"View Reports","path":"payments/payment-button/view-reports","children":[]},{"title":"Subscribe to Webhooks","path":"payments/payment-button/subscribe-to-webhooks","children":[]},{"title":"FAQs","path":"payments/payment-button/faqs","children":[]},{"title":"Glossary","path":"payments/payment-button/glossary","children":[]},{"title":"Subscription Button","path":"","children":[{"title":"About Subscription Button","path":"payments/payment-button/subscription-buttons","children":[]},{"title":"Create and Embed Subscription Button","path":"payments/payment-button/subscription-buttons/embed","children":[]},{"title":"Manage Subscription Buttons","path":"payments/payment-button/subscription-buttons/manage","children":[]},{"title":"View Details and Download Report","path":"payments/payment-button/subscription-buttons/download-reports","children":[]},{"title":"Notifications","path":"payments/payment-button/subscription-buttons/subscribe-to-webhooks","children":[]},{"title":"FAQs","path":"payments/payment-button/subscription-buttons/faqs","children":[]}],"layout":""}],"layout":""},{"title":"Payment Pages","path":"","children":[{"title":"About Payment Pages","path":"payments/payment-pages","children":[]},{"title":"How it Works","path":"","children":[{"title":"How Payment Pages Work","path":"payments/payment-pages/how-it-works","children":[]}],"layout":""},{"title":"Payment Page States","path":"payments/payment-pages/states","children":[]},{"title":"Dashboard","path":"","children":[{"title":"Create a Payment Page","path":"payments/payment-pages/create","children":[]},{"title":"Add Images, Videos and More","path":"payments/payment-pages/add-images-videos","children":[]},{"title":"Manage","path":"","children":[{"title":"Manage Payment Pages","path":"payments/payment-pages/manage","children":[]},{"title":"Customise Payment Pages","path":"payments/payment-pages/customise","children":[]}],"layout":""},{"title":"Configure Payment Receipt","path":"","children":[{"title":"Configure Payment Pages Receipt","path":"payments/payment-pages/receipt","children":[]},{"title":"Configure 80G-Enabled Payment Pages Receipt","path":"payments/payment-pages/80g-receipt","children":[]}],"layout":""},{"title":"Search for a Payment Page","path":"payments/payment-pages/search","children":[]},{"title":"Configure Goal Tracker","path":"payments/payment-pages/goal-tracker","children":[]},{"title":"Add Domain Link (Beta)","path":"payments/payment-pages/domain-linking","children":[]}],"layout":""},{"title":"Payments via Twitter Tip Jar","path":"","children":[{"title":"About Accepting Payments Using Twitter Tip Jar","path":"payments/payment-pages/twitter-tip-jar","children":[]},{"title":"1. Customise Payment Page URL","path":"payments/payment-pages/twitter-tip-jar/customise-url","children":[]},{"title":"2. Link Payment Page to Tip Jar","path":"payments/payment-pages/twitter-tip-jar/link-page","children":[]},{"title":"3. Receive Payments from Followers","path":"payments/payment-pages/twitter-tip-jar/receive-payments","children":[]},{"title":"4. View Settlements on Razorpay Dashboard","path":"payments/payment-pages/twitter-tip-jar/view-settlements","children":[]}],"layout":""},{"title":"Plugins & Add-ons","path":"","children":[{"title":"Track Payments Using Google Tracking ID and Facebook Pixel","path":"payments/payment-pages/plugins-add-ons","children":[]},{"title":"Add Google Analytics Tracking ID","path":"payments/payment-pages/plugins-add-ons/google-analytics","children":[]},{"title":"Add Facebook Pixel","path":"payments/payment-pages/plugins-add-ons/fb-pixel","children":[]},{"title":"Add Facebook Pixel on Payment Success Page","path":"payments/payment-pages/plugins-add-ons/fb-payment-success","children":[]},{"title":"Integrate Payment Pages with Shiprocket","path":"payments/payment-pages/plugins-add-ons/shiprocket","children":[]},{"title":"Integrate Payment Pages with Zapier","path":"payments/payment-pages/plugins-add-ons/zapier","children":[]}],"layout":""},{"title":"View Reports","path":"payments/payment-pages/view-reports","children":[]},{"title":"Subscribe to Webhooks","path":"payments/payment-pages/subscribe-to-webhooks","children":[]},{"title":"FAQs","path":"payments/payment-pages/faqs","children":[]},{"title":"Glossary","path":"payments/payment-pages/glossary","children":[]}],"layout":""},{"title":"Invoices","path":"","children":[{"title":"About Invoices","path":"payments/invoices","children":[]},{"title":"How Invoices Work","path":"payments/invoices/how-it-works","children":[]},{"title":"Invoice States","path":"payments/invoices/states","children":[]},{"title":"Dashboard","path":"","children":[{"title":"Create an Invoice","path":"payments/invoices/create","children":[]},{"title":"Issue an Invoice","path":"payments/invoices/issue","children":[]},{"title":"Search an Invoice","path":"payments/invoices/search","children":[]},{"title":"Update an Invoice","path":"payments/invoices/update","children":[]},{"title":"Resend an Invoice","path":"payments/invoices/resend","children":[]},{"title":"Duplicate an Invoice","path":"payments/invoices/duplicate","children":[]},{"title":"Cancel an Invoice","path":"payments/invoices/cancel","children":[]},{"title":"Delete an Invoice","path":"payments/invoices/delete","children":[]},{"title":"Download and Print an Invoice","path":"payments/invoices/download-print","children":[]}],"layout":""},{"title":"Items","path":"","children":[{"title":"About Items","path":"payments/invoices/items","children":[]},{"title":"Dashboard","path":"payments/invoices/items/dashboard","children":[]}],"layout":""},{"title":"Subscribe to Webhooks","path":"payments/invoices/subscribe-to-webhooks","children":[]},{"title":"Invoice APIs","path":"payments/invoices/apis","children":[]},{"title":"FAQs","path":"payments/invoices/faqs","children":[]},{"title":"Glossary","path":"payments/invoices/glossary","children":[]}],"layout":""},{"title":"QR Codes","path":"","children":[{"title":"About QR Codes","path":"payments/qr-codes","children":[]},{"title":"How QR Codes Work","path":"payments/qr-codes/how-it-works","children":[]},{"title":"QR Code States","path":"payments/qr-codes/states","children":[]},{"title":"Dashboard","path":"","children":[{"title":"Create a QR Code","path":"payments/qr-codes/create","children":[]},{"title":"Search a QR Code","path":"payments/qr-codes/search","children":[]},{"title":"Close a QR Code","path":"payments/qr-codes/close","children":[]}],"layout":""},{"title":"Subscribe to Webhooks","path":"payments/qr-codes/subscribe-to-webhooks","children":[]},{"title":"QR Code APIs","path":"payments/qr-codes/apis","children":[]},{"title":"Migrate from BharatQR to QR Codes","path":"payments/qr-codes/migrate","children":[]},{"title":"View Reports","path":"payments/qr-codes/view-reports","children":[]},{"title":"FAQs","path":"payments/qr-codes/faqs","children":[]},{"title":"Glossary","path":"payments/qr-codes/glossary","children":[]}],"layout":""},{"title":"Affordability","path":"","children":[{"title":"About Affordability Suite","path":"payments/payment-gateway/affordability","children":[]},{"title":"Offers","path":"","children":[{"title":"About Offers","path":"payments/payment-gateway/affordability/offers","children":[]},{"title":"Create Offers","path":"payments/payment-gateway/affordability/offers/create","children":[]},{"title":"Integrate Offers with Standard Checkout","path":"payments/payment-gateway/affordability/offers/standard-integration","children":[]},{"title":"Tutorial - How to Create Offers","path":"payments/payment-gateway/affordability/offers/tutorial","children":[]}],"layout":""},{"title":"No Cost EMI Offers","path":"","children":[{"title":"About No Cost EMI Offers","path":"payments/payment-gateway/affordability/no-cost-emi","children":[]},{"title":"Create No Cost EMI Offers","path":"payments/payment-gateway/affordability/no-cost-emi/create","children":[]},{"title":"Integrate No Cost EMI Offers with Standard Checkout","path":"payments/payment-gateway/affordability/no-cost-emi/standard-integration","children":[]},{"title":"Tutorial - How to Create No Cost EMI Offers","path":"payments/payment-gateway/affordability/no-cost-emi/tutorial","children":[]}],"layout":""},{"title":"Widget","path":"","children":[{"title":"About Affodability Widget","path":"payments/payment-gateway/affordability/widget","children":[]},{"title":"Integrate Affordability Widget with","path":"","children":[{"title":"Native Web(Others)","path":"","children":[{"title":"Integration Steps","path":"payments/payment-gateway/affordability/widget/native-web","children":[]},{"title":"Customisation Options","path":"payments/payment-gateway/affordability/widget/native-web/customise","children":[]}],"layout":""},{"title":"WooCommerce","path":"","children":[{"title":"Integration Steps","path":"payments/payment-gateway/affordability/widget/woocommerce","children":[]},{"title":"Customisation Options","path":"payments/payment-gateway/affordability/widget/woocommerce/customise","children":[]}],"layout":""},{"title":"Shopify","path":"","children":[{"title":"Integration Steps","path":"payments/payment-gateway/affordability/widget/shopify","children":[]},{"title":"Customisation Options","path":"payments/payment-gateway/affordability/widget/shopify/customise","children":[]}],"layout":""}],"layout":""},{"title":"Troubleshooting & FAQs","path":"payments/payment-gateway/affordability/widget/troubleshooting-faqs","children":[]}],"layout":""},{"title":"FAQs","path":"payments/payment-gateway/affordability/faqs","children":[]},{"title":"Glossary","path":"payments/payment-gateway/affordability/glossary","children":[]}],"layout":""},{"title":"Subscriptions","path":"","children":[{"title":"About Subscriptions","path":"payments/subscriptions","children":[]},{"title":"Subscriptions Workflow","path":"payments/subscriptions/workflow","children":[]},{"title":"Subscriptions States","path":"payments/subscriptions/states","children":[]},{"title":"Create Subscriptions","path":"payments/subscriptions/create","children":[]},{"title":"Test Subscriptions","path":"payments/subscriptions/test","children":[]},{"title":"Dashboard","path":"","children":[{"title":"Create and View Plans","path":"payments/subscriptions/create-plans","children":[]},{"title":"Create Subscriptions via Links","path":"payments/subscriptions/create-subscription-links","children":[]},{"title":"Create Add-ons","path":"payments/subscriptions/create-add-ons","children":[]},{"title":"Charge a Card Manually","path":"payments/subscriptions/manually-charge-card","children":[]},{"title":"View a Subscription","path":"payments/subscriptions/view","children":[]},{"title":"Update a Subscription","path":"payments/subscriptions/update","children":[]},{"title":"Pause, Resume and Cancel a Subscription","path":"payments/subscriptions/pause-resume-cancel","children":[]},{"title":"Subscriptions Settings","path":"payments/subscriptions/settings","children":[]}],"layout":""},{"title":"Offers for Subscriptions","path":"","children":[{"title":"About Offers","path":"payments/subscriptions/offers","children":[]},{"title":"Create Subscription Offers","path":"payments/subscriptions/offers/create","children":[]},{"title":"Link an Offer to a Subscription","path":"payments/subscriptions/offers/link","children":[]},{"title":"Update an Offer Linked to a Subscription","path":"payments/subscriptions/offers/update","children":[]},{"title":"Delete an Offer Linked to a Subscription","path":"payments/subscriptions/offers/delete","children":[]}],"layout":""},{"title":"Payment Retries","path":"payments/subscriptions/payment-retries","children":[]},{"title":"Supported Banks and Apps","path":"payments/subscriptions/supported-banks-apps","children":[]},{"title":"Plugins","path":"","children":[{"title":"Woocommerce","path":"","children":[{"title":"Razorpay Subscriptions Plugin for WooCommerce","path":"payments/subscriptions/plugins/woocommerce","children":[]},{"title":"1. Build Integration","path":"payments/subscriptions/plugins/woocommerce/build-integration","children":[]},{"title":"2. Test Integration","path":"payments/subscriptions/plugins/woocommerce/test-integration","children":[]},{"title":"3. Go Live Checklist","path":"payments/subscriptions/plugins/woocommerce/go-live-checklist","children":[]},{"title":"Manage Subscriptions","path":"payments/subscriptions/plugins/woocommerce/manage-subscriptions","children":[]},{"title":"Subscription Status","path":"payments/subscriptions/plugins/woocommerce/subscriptions-status","children":[]}],"layout":""},{"title":"Magento","path":"","children":[{"title":"Razorpay Subscriptions Plugin for Magento","path":"payments/subscriptions/plugins/magento","children":[]},{"title":"Test it out - Sign up for a Subscription","path":"payments/subscriptions/plugins/magento/test-it-out","children":[]},{"title":"Subscription Status","path":"payments/subscriptions/plugins/magento/status","children":[]},{"title":"Manage Subscriptions","path":"payments/subscriptions/plugins/magento/manage","children":[]},{"title":"Webhook Events","path":"payments/subscriptions/plugins/magento/webhook-events","children":[]}],"layout":""},{"title":"OpenCart","path":"","children":[{"title":"Razorpay Subscriptions Plugin for OpenCart","path":"payments/subscriptions/plugins/opencart","children":[]},{"title":"1. Build Integration","path":"payments/subscriptions/plugins/opencart/build-integration","children":[]},{"title":"2. Test Integration","path":"payments/subscriptions/plugins/opencart/test-integration","children":[]},{"title":"3. Go Live Checklist","path":"payments/subscriptions/plugins/opencart/go-live-checklist","children":[]},{"title":"Manage Subscriptions","path":"payments/subscriptions/plugins/opencart/manage-subscriptions","children":[]},{"title":"Subscription Status","path":"payments/subscriptions/plugins/opencart/subscriptions-status","children":[]},{"title":"Webhook Events","path":"payments/subscriptions/plugins/opencart/webhook-events","children":[]}],"layout":""}],"layout":""},{"title":"QR Codes","path":"payments/subscriptions/qr-codes","children":[]},{"title":"Subscribe to Webhooks","path":"payments/subscriptions/subscribe-to-webhooks","children":[]},{"title":"Subscriptions APIs","path":"payments/subscriptions/apis","children":[]},{"title":"Notifications","path":"payments/subscriptions/notifications","children":[]},{"title":"FAQs","path":"payments/subscriptions/faqs","children":[]},{"title":"Glossary","path":"payments/subscriptions/glossary","children":[]}],"layout":""},{"title":"Smart Collect","path":"","children":[{"title":"About Smart Collect","path":"payments/smart-collect","children":[]},{"title":"How Smart Collect Works","path":"payments/smart-collect/how-it-works","children":[]},{"title":"Customer Identifier States","path":"payments/smart-collect/states","children":[]},{"title":"Dashboard","path":"","children":[{"title":"Create Customer Identifiers","path":"payments/smart-collect/create","children":[]},{"title":"Create Customer Identifiers with TPV","path":"payments/smart-collect/create-tpv","children":[]},{"title":"Update Customer Identifier","path":"payments/smart-collect/update","children":[]},{"title":"Close Customer Identifiers","path":"payments/smart-collect/close","children":[]},{"title":"Refund Payments","path":"payments/smart-collect/refund","children":[]},{"title":"Make Test Payments","path":"payments/smart-collect/test-payments","children":[]},{"title":"Search for a Customer Identifier","path":"payments/smart-collect/search","children":[]}],"layout":""},{"title":"Smart Collect APIs","path":"payments/smart-collect/apis","children":[]},{"title":"Smart Collect APIs with TPV","path":"payments/smart-collect/apis-tpv","children":[]},{"title":"Subscribe to Webhooks","path":"payments/smart-collect/subscribe-to-webhooks","children":[]},{"title":"Advanced Options","path":"","children":[{"title":"Refund Failures","path":"payments/smart-collect/refund-failures","children":[]},{"title":"Auto Third-Party Validation (TPV) on Smart Collect","path":"payments/smart-collect/third-party-validation","children":[]}],"layout":""},{"title":"Account Migration - Yes Bank Moratorium","path":"payments/smart-collect/yesbank-moratorium-migration","children":[]},{"title":"Account Migration - New PA/PG Guidelines","path":"payments/smart-collect/pa-pg-migration","children":[]},{"title":"FAQs","path":"payments/smart-collect/faqs","children":[]},{"title":"Glossary","path":"payments/smart-collect/glossary","children":[]}],"layout":""},{"title":"Optimizer","path":"","children":[{"title":"About Optimizer","path":"payments/optimizer","children":[]},{"title":"Get Started with Optimizer","path":"payments/optimizer/get-started","children":[]},{"title":"Add Payment Providers","path":"","children":[{"title":"About Adding Payment Providers","path":"payments/optimizer/add-payment-providers","children":[]},{"title":"PayU","path":"payments/optimizer/payu","children":[]},{"title":"Ingenico","path":"payments/optimizer/ingenico","children":[]},{"title":"PineLabs","path":"payments/optimizer/pinelabs","children":[]},{"title":"Paytm S2S","path":"payments/optimizer/paytm-s2s","children":[]},{"title":"Paytm Instant (beta)","path":"payments/optimizer/paytm-instant","children":[]},{"title":"Cashfree","path":"payments/optimizer/cashfree","children":[]},{"title":"Billdesk","path":"payments/optimizer/billdesk","children":[]},{"title":"CCAvenue","path":"payments/optimizer/ccavenue","children":[]},{"title":"Bank Gateways","path":"payments/optimizer/banks","children":[]}],"layout":""},{"title":"Dynamic Routing","path":"","children":[{"title":"About Dynamic Routing","path":"payments/optimizer/dynamic-routing","children":[]},{"title":"Create Custom Rules","path":"payments/optimizer/create-custom-rule","children":[]},{"title":"Set Rule Priority","path":"payments/optimizer/set-rule-priority","children":[]},{"title":"Update Default Rule","path":"payments/optimizer/update-default-rule","children":[]}],"layout":""},{"title":"SR Analytics Dashboard","path":"payments/optimizer/success-rate","children":[]},{"title":"Capture and Refund Settings","path":"payments/optimizer/capture-refund-settings","children":[]},{"title":"Manage Rules","path":"payments/optimizer/manage-rules","children":[]},{"title":"Single Reconciliation View","path":"payments/optimizer/reconciliation","children":[]},{"title":"Roles and Permissions","path":"payments/optimizer/roles-and-permissions","children":[]},{"title":"Supported Gateways and Aggregators","path":"payments/optimizer/supported-gateways-aggregators","children":[]},{"title":"Tokenisation for Optimizer","path":"payments/optimizer/tokenisation","children":[]},{"title":"FAQs","path":"payments/optimizer/faqs","children":[]}],"layout":""},{"title":"Route","path":"","children":[{"title":"About Route","path":"payments/route","children":[]},{"title":"Route Use Cases","path":"payments/route/use-cases","children":[]},{"title":"Linked Accounts","path":"payments/route/linked-account","children":[]},{"title":"Dashboard","path":"","children":[{"title":"Batch Upload for Linked Accounts and Transfers","path":"payments/route/batch-upload","children":[]},{"title":"Transfer Funds to Linked Accounts","path":"payments/route/transfer-funds-to-linked-accounts","children":[]},{"title":"Schedule Settlements","path":"payments/route/schedule-settlement","children":[]},{"title":"Payment Reversals","path":"payments/route/reversal","children":[]},{"title":"Refund to Customers","path":"payments/route/refund","children":[]}],"layout":""},{"title":"Transfers and Related Fees","path":"payments/route/transfer-fees-example","children":[]},{"title":"Linked Account Dashboard","path":"","children":[{"title":"Initiate Refund","path":"payments/route/linked-account/initiate-refund","children":[]},{"title":"Reversals and Settlements","path":"payments/route/linked-account/reversals-settlements","children":[]},{"title":"Manage Profile and Team","path":"payments/route/linked-account/manage-profile","children":[]}],"layout":""},{"title":"Plugins","path":"","children":[{"title":"Razorpay Route Module for WooCommerce","path":"payments/route/plugins/woocommerce","children":[]},{"title":"1. Build Integration","path":"","children":[{"title":"Transfers via Orders or Payments","path":"payments/route/plugins/woocommerce/build-integration/transfers-orders-payments","children":[]},{"title":"Direct Transfers","path":"payments/route/plugins/woocommerce/build-integration/direct-transfers","children":[]}],"layout":""},{"title":"2. Test Integration","path":"payments/route/plugins/woocommerce/test-integration","children":[]},{"title":"3. Go-live Checklist","path":"payments/route/plugins/woocommerce/go-live-checklist","children":[]},{"title":"Create Reversals","path":"payments/route/plugins/woocommerce/create-reversals","children":[]}],"layout":""},{"title":"View Reports","path":"payments/route/view-reports","children":[]},{"title":"Subscribe to Webhooks","path":"payments/route/subscribe-to-webhooks","children":[]},{"title":"Route APIs","path":"payments/route/apis","children":[]},{"title":"FAQs","path":"payments/route/faqs","children":[]},{"title":"Glossary","path":"payments/route/glossary","children":[]}],"layout":""},{"title":"Third Party Validation","path":"","children":[{"title":"Third Party Validation on Razorpay Standard Integration","path":"payments/third-party-validation","children":[]},{"title":"Best Practices","path":"payments/third-party-validation/best-practices","children":[]},{"title":"Supported Banks","path":"payments/third-party-validation/bank-list","children":[]}],"layout":""},{"title":"Payments Mobile App","path":"","children":[{"title":"About Razorpay Payments Mobile App","path":"payments/mobile-app","children":[]},{"title":"Get Started","path":"payments/mobile-app/get-started","children":[]},{"title":"Accept Payments","path":"","children":[{"title":"Payment Links","path":"payments/mobile-app/accept-payments/payment-links","children":[]},{"title":"Payment Pages","path":"payments/mobile-app/accept-payments/payment-pages","children":[]},{"title":"Razorpay.me URL","path":"","children":[{"title":"About Accepting Payments Using Razorpay.me","path":"payments/mobile-app/accept-payments/razorpay-me","children":[]},{"title":"Manage","path":"payments/mobile-app/accept-payments/razorpay-me/manage","children":[]}],"layout":""},{"title":"Payment Gateway","path":"payments/mobile-app/accept-payments/payment-gateway","children":[]}],"layout":""},{"title":"Track and Manage","path":"","children":[{"title":"Payments","path":"payments/mobile-app/track-manage","children":[]},{"title":"Issue Refunds","path":"payments/mobile-app/track-manage/issue-refunds","children":[]},{"title":"View Settlements","path":"payments/mobile-app/track-manage/view-settlements","children":[]}],"layout":""},{"title":"Roles and Permissions","path":"payments/mobile-app/roles-and-permissions","children":[]},{"title":"Settings","path":"payments/mobile-app/settings","children":[]},{"title":"FAQs","path":"payments/mobile-app/faqs","children":[]},{"title":"Glossary","path":"payments/mobile-app/glossary","children":[]}],"layout":""},{"title":"ePOS App (Deprecated)","path":"payments/epos-app","children":[]},{"title":"Thirdwatch (Deprecated)","path":"payments/thirdwatch","children":[]},{"title":"Glossary","path":"payments/glossary","children":[]}]},{"title":"Banking Plus","path":"/x","iconName":"bank","children":[{"title":"RazorpayX","path":"x","children":[]},{"title":"Sign Up","path":"","children":[{"title":"Create a RazorpayX Account","path":"x/sign-up","children":[]},{"title":"Account Types","path":"","children":[{"title":"About Account Types","path":"x/account-types","children":[]},{"title":"RazorpayX Lite","path":"x/account-types/razorpayx-lite","children":[]},{"title":"RazorpayX - Current Account","path":"","children":[{"title":"About RazorpayX - Current Account","path":"x/account-types/current-account","children":[]},{"title":"ICICI","path":"","children":[{"title":"Private / Public Limited Company","path":"x/icici-current-account/company","children":[]},{"title":"Sole Proprietorship","path":"x/icici-current-account/sole-proprietorship","children":[]},{"title":"Limited Liability Partnership","path":"x/icici-current-account/llp","children":[]},{"title":"Partnership","path":"x/icici-current-account/partnership","children":[]},{"title":"KYC","path":"x/icici-current-account/entity-address-proof","children":[]}],"layout":""},{"title":"RBL","path":"","children":[{"title":"Private / Public Limited Company","path":"x/rbl-current-account/company","children":[]},{"title":"Sole Proprietorship","path":"x/rbl-current-account/sole-proprietorship","children":[]},{"title":"Limited Liability Partnership","path":"x/rbl-current-account/llp","children":[]},{"title":"Partnership","path":"x/rbl-current-account/partnership","children":[]},{"title":"Trust or Society","path":"x/rbl-current-account/trust-society","children":[]},{"title":"KYC","path":"x/rbl-current-account/cif","children":[]}],"layout":""}],"layout":""},{"title":"Source Account Validation","path":"x/account-types/source-account-validation","children":[]},{"title":"FAQs","path":"x/account-types/faqs","children":[]}],"layout":""}],"layout":""},{"title":"Dashboard","path":"","children":[{"title":"About Dashboard","path":"x/dashboard","children":[]},{"title":"Generate API Keys","path":"x/dashboard/api-keys","children":[]},{"title":"Allowlist IPs","path":"x/dashboard/allowlist-ip","children":[]},{"title":"Test Mode","path":"x/dashboard/test-mode","children":[]},{"title":"Keyboard Shortcuts","path":"x/dashboard/keyboard-shortcuts","children":[]},{"title":"Global Search","path":"x/dashboard/global-search","children":[]},{"title":"Contact Support","path":"x/support","children":[]},{"title":"Account Settings","path":"","children":[{"title":"Manage Teams","path":"x/manage-teams","children":[]},{"title":"Create User Roles","path":"x/manage-teams/create-user-role","children":[]},{"title":"Approval Workflow","path":"x/manage-teams/approval-workflow-changes","children":[]},{"title":"Billing - Fees and Taxes","path":"x/manage-teams/billing","children":[]},{"title":"Two-Factor Authentication","path":"x/manage-teams/2fa","children":[]},{"title":"Credits and Free Payouts","path":"x/manage-teams/credits-free-payouts","children":[]},{"title":"Chartered Accountant Portal","path":"x/manage-teams/ca-portal","children":[]},{"title":"FAQs","path":"x/manage-teams/faqs","children":[]}],"layout":""},{"title":"FAQs","path":"x/dashboard/faqs","children":[]}],"layout":""},{"title":"Account Statement","path":"","children":[{"title":"About Account Statement","path":"x/account-statement","children":[]},{"title":"Integrate","path":"","children":[{"title":"Sync Account Statements","path":"x/account-statement/integrate","children":[]},{"title":"Zoho Books","path":"x/account-statement/integrate/zohobooks","children":[]},{"title":"Tally","path":"x/account-statement/integrate/tally","children":[]},{"title":"QuickBooks","path":"x/account-statement/integrate/quickbooks","children":[]}],"layout":""},{"title":"Reports","path":"x/account-statement/report","children":[]},{"title":"APIs","path":"x/account-statement/api","children":[]}],"layout":""},{"title":"Contacts","path":"","children":[{"title":"About Contacts","path":"x/contacts","children":[]},{"title":"Contact Bulk Uploads","path":"x/contacts/bulk-uploads","children":[]},{"title":"APIs","path":"x/contacts/api","children":[]},{"title":"FAQs","path":"x/contacts/faqs","children":[]}],"layout":""},{"title":"Fund Accounts","path":"","children":[{"title":"About Fund Accounts","path":"x/fund-accounts","children":[]},{"title":"Fund Account Validation","path":"x/fund-account-validation","children":[]},{"title":"APIs","path":"x/fund-accounts/api","children":[]},{"title":"FAQs","path":"x/fund-accounts/faqs","children":[]}],"layout":""},{"title":"Payouts","path":"","children":[{"title":"About Payouts","path":"x/payouts","children":[]},{"title":"Payout States and Life Cycle","path":"x/payouts/states-life-cycle","children":[]},{"title":"Types of Payouts","path":"","children":[{"title":"Intelligent Payouts","path":"x/payouts/intelligent-payouts","children":[]},{"title":"Queued Payouts","path":"x/payouts/queued","children":[]},{"title":"Scheduled Payouts","path":"x/payouts/scheduled","children":[]}],"layout":""},{"title":"Payouts to Cards","path":"x/payouts/cards","children":[]},{"title":"Sub-Accounts","path":"x/payouts/sub-accounts","children":[]},{"title":"Payouts Best Practices","path":"x/payouts/best-practices","children":[]},{"title":"Reports","path":"x/payouts/reports","children":[]},{"title":"APIs","path":"x/payouts/api","children":[]},{"title":"FAQs","path":"x/payouts/faqs","children":[]},{"title":"Bulk Payouts","path":"","children":[{"title":"About Bulk Payouts","path":"x/bulk-payouts","children":[]},{"title":"Bulk Payouts Life Cycle","path":"x/bulk-payouts/life-cycle","children":[]},{"title":"Bulk Upload Status","path":"x/bulk-payouts/uploads","children":[]},{"title":"Bulk Upload Report","path":"x/bulk-payouts/report","children":[]}],"layout":""},{"title":"Wallet","path":"","children":[{"title":"About Amazon Payout Gift Card","path":"x/payout-wallet/amazon","children":[]},{"title":"Amazon Branding Guidelines","path":"x/payout-wallet/amazon/branding-guidelines","children":[]},{"title":"APIs","path":"x/payout-wallet/amazon/api","children":[]}],"layout":""}],"layout":""},{"title":"Vendor Payments","path":"","children":[{"title":"About Vendor Payments","path":"x/vendor-payments","children":[]},{"title":"Invoices","path":"","children":[{"title":"Life Cycle","path":"x/vendor-payments/life-cycle","children":[]},{"title":"Add Invoice","path":"x/vendor-payments/invoices","children":[]},{"title":"Add Invoices in Bulk","path":"x/vendor-payments/bulk-invoices","children":[]},{"title":"Invoice Report","path":"x/vendor-payments/invoice-report","children":[]}],"layout":""},{"title":"Vendor Payouts","path":"","children":[{"title":"Partial Payouts","path":"x/vendor-payments/partial-payouts","children":[]},{"title":"Scheduled Payouts","path":"x/vendor-payments/scheduled-payouts","children":[]},{"title":"Bulk Payments","path":"x/vendor-payments/bulk","children":[]}],"layout":""},{"title":"Accounting Integrations","path":"","children":[{"title":"About Accounting Integrations","path":"x/vendor-payments/integrations","children":[]},{"title":"QuickBooks Integration","path":"x/vendor-payments/quickbooks-integration","children":[]},{"title":"Zoho Books Integration","path":"","children":[{"title":"About Zoho Books","path":"x/vendor-payments/zohobooks","children":[]},{"title":"Integrate RazorpayX with Zoho Books","path":"x/vendor-payments/zohobooks/integrate","children":[]},{"title":"Sync RazorpayX with Zoho Books","path":"x/vendor-payments/zohobooks/sync-zohobooks","children":[]}],"layout":""},{"title":"Tally Bidirectional Integration","path":"","children":[{"title":"About RazorpayX-Tally Integration","path":"x/vendor-payments/tally","children":[]},{"title":"Set Up Integration","path":"x/vendor-payments/tally/set-up","children":[]},{"title":"Sync Purchase Vouchers","path":"x/vendor-payments/tally/sync-purchase-vouchers","children":[]},{"title":"Sync Payment Vouchers","path":"x/vendor-payments/tally/sync-payment-vouchers","children":[]},{"title":"Bring Invoices to Tally","path":"x/vendor-payments/tally/bring-bills","children":[]},{"title":"Smart Bank Statement Sync","path":"x/vendor-payments/tally/bank-statement-sync","children":[]}],"layout":""}],"layout":""},{"title":"Tally e-Payments","path":"","children":[{"title":"About Tally e-Payments","path":"x/tally-epayments","children":[]},{"title":"Set Up e-Payments","path":"x/tally-epayments/set-up","children":[]},{"title":"Export and Approve Payouts","path":"x/tally-epayments/export-approve-payouts","children":[]},{"title":"Reconcile Payouts","path":"x/tally-epayments/reconcile-payouts","children":[]}],"layout":""},{"title":"Vendor Portal","path":"x/vendor-payments/portal/business","children":[]},{"title":"FAQs","path":"x/vendor-payments/faqs","children":[]}],"layout":""},{"title":"Tax Payments","path":"","children":[{"title":"About Tax Payments","path":"x/tax-payments","children":[]},{"title":"Tax Payment Life Cycle","path":"x/tax-payments/life-cycle","children":[]},{"title":"Automatic TDS","path":"x/tax-payments/automatic-tds","children":[]},{"title":"Advance Tax Payments","path":"x/tax-payments/advance","children":[]},{"title":"Goods and Services Tax (GST)","path":"x/tax-payments/gst","children":[]}],"layout":""},{"title":"Payout Links","path":"","children":[{"title":"About Payout Links","path":"x/payout-links","children":[]},{"title":"Payout Links Life Cycle","path":"x/payout-links/life-cycle","children":[]},{"title":"Dashboard Actions","path":"","children":[{"title":"Create Payout Links","path":"x/payout-links/create","children":[]},{"title":"Set Payout Links Expiry","path":"x/payout-links/set-expiry","children":[]}],"layout":""},{"title":"Shopify Payout Links","path":"x/payout-links/shopify","children":[]},{"title":"Bulk Payout Links","path":"","children":[{"title":"Create Bulk Payout Links","path":"x/payout-links/bulk","children":[]},{"title":"Bulk Report and Errors","path":"x/payout-links/report-and-errors","children":[]}],"layout":""},{"title":"Reports","path":"x/payout-links/reports","children":[]},{"title":"APIs","path":"x/payout-links/api","children":[]},{"title":"FAQs","path":"x/payout-links/faqs","children":[]}],"layout":""},{"title":"Reports","path":"","children":[{"title":"About Reports","path":"x/reports","children":[]}],"layout":""},{"title":"APIs and Webhooks","path":"","children":[{"title":"APIs","path":"x/apis","children":[]},{"title":"About Webhooks","path":"x/webhooks","children":[]},{"title":"Subscribe to Webhooks","path":"x/webhooks/subscribe","children":[]}],"layout":""},{"title":"Razorpay Capital","path":"","children":[{"title":"About Razorpay Capital","path":"x/capital","children":[]},{"title":"Line of Credit","path":"","children":[{"title":"About Line of Credit","path":"x/capital/line-of-credit","children":[]},{"title":"Make Withdrawals & Repayments","path":"x/capital/line-of-credit/dashboard","children":[]}],"layout":""},{"title":"Corporate Cards","path":"x/capital/corporate-cards","children":[]},{"title":"FAQs","path":"x/capital/faqs","children":[]}],"layout":""},{"title":"RazorpayX Payroll","path":"","children":[{"title":"About RazorpayX Payroll","path":"x/xpayroll","children":[]},{"title":"Plans","path":"x/xpayroll/plans","children":[]},{"title":"Employers","path":"","children":[{"title":"Account Setup","path":"x/xpayroll/employers/setup/account","children":[]},{"title":"Payroll Checklist","path":"x/xpayroll/employers/setup/execute-payroll","children":[]},{"title":"Salary","path":"","children":[{"title":"About Salary","path":"x/xpayroll/employers/salary","children":[]},{"title":"Run Payroll","path":"x/xpayroll/employers/salary/run-payroll","children":[]},{"title":"One-time Payments","path":"x/xpayroll/employers/salary/one-time-payments","children":[]},{"title":"Reimbursements","path":"x/xpayroll/employers/salary/reimbursements","children":[]},{"title":"Exceptional Cases","path":"x/xpayroll/employers/salary/exceptional-cases","children":[]}],"layout":""},{"title":"Statutory Compliance","path":"","children":[{"title":"About Statutory Compliance","path":"x/xpayroll/employers/setup/statutory-compliance","children":[]},{"title":"Tax Deducted at Source (TDS)","path":"","children":[{"title":"Deduct TDS","path":"x/xpayroll/employers/setup/tds","children":[]},{"title":"Verify TDS","path":"x/xpayroll/employers/setup/tds/verify","children":[]}],"layout":""},{"title":"Provident Fund","path":"","children":[{"title":"About Provident Fund","path":"x/xpayroll/employers/setup/provident-fund","children":[]},{"title":"Register PF","path":"x/xpayroll/employers/setup/provident-fund/register","children":[]}],"layout":""},{"title":"Professional Tax","path":"x/xpayroll/employers/setup/pt","children":[]}],"layout":""},{"title":"Leaves & Attendance","path":"","children":[{"title":"Leaves","path":"x/xpayroll/employers/human-resources/leaves","children":[]},{"title":"Attendance","path":"x/xpayroll/employers/human-resources/attendance","children":[]}],"layout":""},{"title":"Administrator Role","path":"","children":[{"title":"HR Operations","path":"x/xpayroll/employers/human-resources","children":[]},{"title":"Documents & Letters","path":"x/xpayroll/employers/human-resources/documents-letters","children":[]},{"title":"Payroll Payouts","path":"x/xpayroll/employers/payroll-payouts","children":[]}],"layout":""}],"layout":""},{"title":"Employees","path":"","children":[{"title":"Employee Dashboard","path":"x/xpayroll/employees","children":[]},{"title":"Leaves","path":"x/xpayroll/employees/leaves","children":[]},{"title":"Reimbursements","path":"x/xpayroll/employees/reimbursements","children":[]},{"title":"IT Declarations","path":"x/xpayroll/employees/declarations","children":[]},{"title":"Resignation","path":"x/xpayroll/employees/resignation","children":[]}],"layout":""},{"title":"Integrate","path":"","children":[{"title":"About Integrations","path":"x/xpayroll/integrate","children":[]},{"title":"Current Account","path":"x/xpayroll/integrate/current-account","children":[]},{"title":"Insurance","path":"x/xpayroll/integrate/insurance","children":[]},{"title":"Slack","path":"x/xpayroll/integrate/slack","children":[]},{"title":"WhatsApp","path":"x/xpayroll/integrate/whatsapp","children":[]}],"layout":""}],"layout":""},{"title":"Glossary","path":"x/glossary","children":[]}]},{"title":"Partners","path":"/partners","iconName":"user","children":[{"title":"Razorpay Partners","path":"partners","children":[]},{"title":"Become a Razorpay Partner","path":"","children":[{"title":"New Merchants","path":"partners/new-merchant","children":[]},{"title":"Existing Merchants","path":"partners/existing-merchant","children":[]}],"layout":""},{"title":"Earnings","path":"","children":[{"title":"Commission for Payment products","path":"partners/commissions","children":[]},{"title":"Referral Bonus for X Current Accounts","path":"partners/commissions/referral-bonus","children":[]},{"title":"Commission Settlement Process","path":"partners/commissions/settlement-process","children":[]},{"title":"Commission Reports and Auto-generated Invoices","path":"partners/commissions/reports-invoices","children":[]}],"layout":""},{"title":"Resellers","path":"","children":[{"title":"About Resellers","path":"partners/resellers","children":[]},{"title":"Add Sub-merchants","path":"partners/resellers/add-submerchants","children":[]},{"title":"Activation States","path":"partners/resellers/activation-status","children":[]},{"title":"Perform KYC","path":"partners/resellers/perform-kyc","children":[]}],"layout":""},{"title":"Aggregators","path":"","children":[{"title":"About Aggregators","path":"partners/aggregators","children":[]},{"title":"Become an Aggregator","path":"partners/aggregators/become-aggregator","children":[]},{"title":"Add Submerchants","path":"","children":[{"title":"Using Dashboard","path":"partners/aggregators/add-submerchants","children":[]},{"title":"Using APIs","path":"","children":[{"title":"Sub-Merchant Onboarding APIs","path":"partners/aggregators/onboarding-api","children":[]},{"title":"Workflow","path":"partners/aggregators/onboarding-api/workflow","children":[]},{"title":"Webhooks","path":"partners/aggregators/onboarding-api/webhooks","children":[]},{"title":"Product Activation","path":"partners/aggregators/onboarding-api/product-activation","children":[]},{"title":"Appendix","path":"partners/aggregators/onboarding-api/appendix","children":[]}],"layout":""}],"layout":""},{"title":"Partner Auth","path":"","children":[{"title":"About Partner Auth","path":"partners/aggregators/partner-auth","children":[]},{"title":"Payment Gateway","path":"partners/aggregators/partner-auth/payment-gateway","children":[]},{"title":"Payment Links","path":"partners/aggregators/partner-auth/payment-links","children":[]},{"title":"QR Codes","path":"partners/aggregators/partner-auth/qr-codes","children":[]},{"title":"Smart Collect","path":"partners/aggregators/partner-auth/smart-collect","children":[]},{"title":"Subscriptions","path":"partners/aggregators/partner-auth/subscriptions","children":[]},{"title":"Token Sharing for Partner Auth Model","path":"partners/aggregators/partner-auth/token-sharing","children":[]},{"title":"Recurring Payments","path":"","children":[{"title":"About Recurring Payments for Partners","path":"partners/aggregators/partner-auth/recurring-payments","children":[]},{"title":"Emandate","path":"","children":[{"title":"1. Emandate Registration","path":"partners/aggregators/partner-auth/recurring-payments/emandate/registration","children":[]},{"title":"2. Fetch and Manage Tokens","path":"partners/aggregators/partner-auth/recurring-payments/emandate/fetch-manage-tokens","children":[]},{"title":"3. Create Subsequent Payments","path":"partners/aggregators/partner-auth/recurring-payments/emandate/create-subsequent-payments","children":[]}],"layout":""},{"title":"Cards","path":"","children":[{"title":"1. Create Authorisation Transaction","path":"partners/aggregators/partner-auth/recurring-payments/cards/create-authorisation-transaction","children":[]},{"title":"2. Fetch and Manage Tokens","path":"partners/aggregators/partner-auth/recurring-payments/cards/fetch-manage-tokens","children":[]},{"title":"3. Create Subsequent Payments","path":"partners/aggregators/partner-auth/recurring-payments/cards/create-subsequent-payments","children":[]}],"layout":""},{"title":"UPI","path":"","children":[{"title":"1. Create Authorisation Transaction","path":"partners/aggregators/partner-auth/recurring-payments/upi/create-authorisation-transaction","children":[]},{"title":"2. Fetch and Manage Tokens","path":"partners/aggregators/partner-auth/recurring-payments/upi/fetch-manage-tokens","children":[]},{"title":"3. Create Subsequent Payments","path":"partners/aggregators/partner-auth/recurring-payments/upi/create-subsequent-payments","children":[]}],"layout":""},{"title":"UPI With TPV","path":"","children":[{"title":"1. Create Authorisation Transaction","path":"partners/aggregators/partner-auth/recurring-payments/upi-tpv/create-authorisation-transaction","children":[]},{"title":"2. Fetch and Manage Tokens","path":"partners/aggregators/partner-auth/recurring-payments/upi-tpv/fetch-manage-tokens","children":[]},{"title":"3. Create Subsequent Payments","path":"partners/aggregators/partner-auth/recurring-payments/upi-tpv/create-subsequent-payments","children":[]}],"layout":""}],"layout":""}],"layout":""},{"title":"Testing Operations","path":"partners/aggregators/testing","children":[]}],"layout":""},{"title":"Razorpay for Platforms and Marketplaces","path":"","children":[{"title":"About Razorpay for Platforms and Marketplaces","path":"partners/platforms-and-marketplaces","children":[]},{"title":"Become a Platform Partner","path":"partners/platforms-and-marketplaces/become-platform-partner","children":[]},{"title":"Onboard Businesses","path":"","children":[{"title":"About Onboarding Businesses","path":"partners/platforms-and-marketplaces/onboard-businesses","children":[]},{"title":"Integrate OAuth","path":"","children":[{"title":"About OAuth","path":"partners/platforms-and-marketplaces/onboard-businesses/integrate-oauth","children":[]},{"title":"1. Build Integration","path":"partners/platforms-and-marketplaces/onboard-businesses/integrate-oauth/integration-steps","children":[]},{"title":"2. Test Integration","path":"partners/platforms-and-marketplaces/onboard-businesses/integrate-oauth/test-integration","children":[]},{"title":"3. Go-live Checklist","path":"partners/platforms-and-marketplaces/onboard-businesses/integrate-oauth/go-live-checklist","children":[]},{"title":"Subscribe to Webhooks","path":"partners/platforms-and-marketplaces/onboard-businesses/integrate-oauth/subscribe-to-webhooks","children":[]},{"title":"Revoke Access to Application","path":"partners/platforms-and-marketplaces/onboard-businesses/integrate-oauth/revoke-access","children":[]}],"layout":""},{"title":"Customise Onboarding","path":"partners/platforms-and-marketplaces/onboard-businesses/customise-onboarding","children":[]}],"layout":""},{"title":"Process Payments","path":"partners/platforms-and-marketplaces/process-payments","children":[]},{"title":"Control of Funds","path":"","children":[{"title":"About Control of Funds","path":"partners/platforms-and-marketplaces/control-of-funds","children":[]},{"title":"Set up Platform and Third-Party Accounts","path":"partners/platforms-and-marketplaces/control-of-funds/set-up-accounts","children":[]},{"title":"Process Platform and Third-Party Fees","path":"partners/platforms-and-marketplaces/control-of-funds/process-fees","children":[]},{"title":"Refunds and Reversals","path":"partners/platforms-and-marketplaces/control-of-funds/refunds-and-reversals","children":[]}],"layout":""},{"title":"Reports and Reconciliation","path":"","children":[{"title":"Platform","path":"partners/platforms-and-marketplaces/reports-and-reconciliation/platform","children":[]},{"title":"Sub-merchants","path":"partners/platforms-and-marketplaces/reports-and-reconciliation/sub-merchant","children":[]},{"title":"Third-Party Service Providers","path":"partners/platforms-and-marketplaces/reports-and-reconciliation/third-party","children":[]}],"layout":""}],"layout":""},{"title":"Capital","path":"partners/capital","children":[]},{"title":"FAQs","path":"partners/faqs","children":[]},{"title":"Glossary","path":"partners/glossary","children":[]}]},{"title":"Developer Tools","path":"/api","iconName":"dev-sign","children":[{"title":"API Reference Guide","children":[{"title":"Get Started with APIs","path":"","children":[{"title":"Introduction","path":"api","children":[]},{"title":"API Basics","path":"api/basics","children":[]},{"title":"Authentication & Sandbox Setup","path":"api/authentication","children":[]},{"title":"Structure & Pagination","path":"","children":[{"title":"Entity & Metadata","path":"api/entity-metadata","children":[]},{"title":"Pagination & Rate Limiting","path":"api/pagination","children":[]}],"layout":""},{"title":"Best Practices","path":"api/best-practices","children":[]},{"title":"Glossary","path":"api/glossary","children":[]}],"layout":""},{"title":"Orders","path":"api/orders","children":[],"layout":"api"},{"title":"Payments","path":"","children":[{"title":"Payments","path":"api/payments","children":[],"layout":"api"},{"title":"Downtime","path":"api/payments/downtime","children":[],"layout":"api"}],"layout":""},{"title":"Settlements","path":"","children":[{"title":"Settlements","path":"api/settlements","children":[],"layout":"api"},{"title":"Instant Settlements","path":"api/settlements/instant","children":[],"layout":"api"}],"layout":""},{"title":"Refunds","path":"api/refunds","children":[],"layout":"api"},{"title":"Disputes","path":"","children":[{"title":"Disputes","path":"api/disputes","children":[],"layout":"api"},{"title":"Documents","path":"api/documents","children":[],"layout":"api"}],"layout":""},{"title":"Customers","path":"api/customers","children":[],"layout":"api"},{"title":"Payments Suite","path":"","children":[{"title":"Payment Links","path":"","children":[{"title":"Payment Links","path":"api/payments/payment-links","children":[],"layout":"api"},{"title":"Customise","path":"","children":[{"title":"About Payment Links Customisation","path":"api/payments/payment-links/customise","children":[]},{"title":"Implement Thematic Changes in Payment Links Checkout Section","path":"api/payments/payment-links/checkout-theme","children":[],"layout":"api"},{"title":"Change Business Name","path":"api/payments/payment-links/change-business-name","children":[],"layout":"api"},{"title":"Customise Payment Methods","path":"api/payments/payment-links/customise-payment-methods","children":[],"layout":"api"},{"title":"Rename Labels in Checkout Section","path":"api/payments/payment-links/rename-checkout-labels","children":[],"layout":"api"},{"title":"Rename Labels in Payment Details Section","path":"api/payments/payment-links/rename-payment-details-labels","children":[],"layout":"api"}],"layout":""},{"title":"Advanced Options","path":"","children":[{"title":"About Advanced Options","path":"api/payments/payment-links/advanced-options","children":[]},{"title":"Receive Payments via Bank Transfer","path":"api/payments/payment-links/receive-bank-transfer-payments","children":[]},{"title":"Offers on Payment Links","path":"api/payments/payment-links/offers","children":[]},{"title":"Managing Reminders for Payment Links","path":"api/payments/payment-links/reminders","children":[]},{"title":"Transfer Payments Received Using Payment Links","path":"api/payments/payment-links/transfer-payments","children":[],"layout":"api"},{"title":"Perform Third-Party Validation Using Payment Links","path":"api/payments/payment-links/third-party-validation","children":[],"layout":"api"}],"layout":""}],"layout":""},{"title":"QR Codes","path":"","children":[{"title":"QR Codes","path":"api/qr-codes","children":[],"layout":"api"},{"title":"Image Content","path":"","children":[{"title":"QR Codes (with Image Content)","path":"api/qr-codes/image-content","children":[],"layout":"api"},{"title":"Best Practices for Image Content Integration","path":"api/qr-codes/image-content/best-practices","children":[]}],"layout":""}],"layout":""},{"title":"Invoices","path":"api/payments/invoices","children":[],"layout":"api"},{"title":"Items","path":"api/payments/items","children":[],"layout":"api"},{"title":"Subscriptions","path":"api/payments/subscriptions","children":[],"layout":"api"},{"title":"Route","path":"","children":[{"title":"Route","path":"api/payments/route","children":[],"layout":"api"},{"title":"Linked Account Onboarding","path":"api/payments/route/linked-account-onboarding","children":[],"layout":"api"},{"title":"Route Transfers","path":"api/payments/route/transfers","children":[],"layout":"api"},{"title":"Appendix","path":"api/payments/route/appendix","children":[]}],"layout":""},{"title":"Smart Collect","path":"","children":[{"title":"Smart Collect","path":"api/payments/smart-collect","children":[],"layout":"api"},{"title":"Smart Collect with TPV","path":"api/payments/smart-collect-tpv","children":[],"layout":"api"}],"layout":""}],"layout":""},{"title":"Partners","path":"","children":[{"title":"Sub-Merchant Onboarding","path":"api/partners","children":[]},{"title":"Account","path":"api/partners/account-onboarding","children":[],"layout":"api"},{"title":"Product Configuration","path":"api/partners/product-configuration","children":[],"layout":"api"},{"title":"Stakeholder","path":"api/partners/stakeholder","children":[],"layout":"api"},{"title":"Terms and Conditions","path":"api/partners/terms-conditions","children":[],"layout":"api"},{"title":"Document","path":"api/partners/upload-document","children":[],"layout":"api"},{"title":"Webhooks","path":"api/partners/webhooks","children":[],"layout":"api"},{"title":"Generic API Errors","path":"api/partners/errors","children":[],"layout":"api"}],"layout":""},{"title":"RazorpayX","path":"","children":[{"title":"Get Started","path":"api/x","children":[],"layout":"api"},{"title":"Account Validation","path":"api/x/account-validation","children":[],"layout":"api"},{"title":"Contacts","path":"api/x/contacts","children":[],"layout":"api"},{"title":"Fund Accounts","path":"api/x/fund-accounts","children":[],"layout":"api"},{"title":"Payouts","path":"api/x/payouts","children":[],"layout":"api"},{"title":"Payouts to Cards","path":"api/x/payouts-cards","children":[],"layout":"api"},{"title":"Payout Composite","path":"api/x/payout-composite","children":[],"layout":"api"},{"title":"Payout Idempotency","path":"api/x/payout-idempotency","children":[],"layout":"api"},{"title":"Payout Links","path":"api/x/payout-links","children":[],"layout":"api"},{"title":"Payout Wallet - Amazon","path":"api/x/payout-wallet","children":[],"layout":"api"},{"title":"Transactions","path":"api/x/transactions","children":[],"layout":"api"},{"title":"Webhooks","path":"api/x/webhooks","children":[]}],"layout":""}]},{"title":"Errors","children":[{"title":"About Error Codes","path":"api/errors","children":[]},{"title":"List","path":"api/errors/list","children":[]},{"title":"Payment Methods","path":"api/errors/payment-methods","children":[]},{"title":"RazorpayX","path":"","children":[{"title":"About Error Codes","path":"api/errors/x","children":[]},{"title":"Contact","path":"api/errors/x/contacts","children":[]},{"title":"Fund Account","path":"api/errors/x/fund-account","children":[]},{"title":"Payouts Status Details","path":"api/errors/x/payout-status-details","children":[]}],"layout":""}]},{"title":"Webhooks","children":[{"title":"Webhooks","path":"webhooks","children":[]},{"title":"Set Up and Edit Webhooks","path":"","children":[{"title":"Payments","path":"webhooks/setup-edit-payments","children":[]},{"title":"RazorpayX","path":"webhooks/setup-edit-x","children":[]}],"layout":""},{"title":"Best Practices","path":"webhooks/best-practices","children":[]},{"title":"Validate and Test Webhooks","path":"webhooks/validate-test","children":[]},{"title":"Sample Payload","path":"","children":[{"title":"Orders","path":"webhooks/payloads/orders","children":[]},{"title":"Payments","path":"webhooks/payloads/payments","children":[]},{"title":"Refunds","path":"webhooks/payloads/refunds","children":[]},{"title":"Disputes","path":"webhooks/payloads/disputes","children":[]},{"title":"Invoices","path":"webhooks/payloads/invoices","children":[]},{"title":"Subscriptions","path":"webhooks/payloads/subscriptions","children":[]},{"title":"Partners","path":"","children":[{"title":"OAuth","path":"","children":[{"title":"OAuth Partner - Sample Payload","path":"webhooks/payloads/partners/oauth","children":[]}],"layout":""},{"title":"Aggregator","path":"","children":[{"title":"Sub-merchant Onboarding Events","path":"webhooks/payloads/partners","children":[]},{"title":"Activated","path":"webhooks/payloads/partners/activated","children":[]},{"title":"Under Review","path":"webhooks/payloads/partners/under-review","children":[]},{"title":"Needs Clarification","path":"webhooks/payloads/partners/needs-clarification","children":[]},{"title":"Suspended","path":"webhooks/payloads/partners/suspended","children":[]},{"title":"Rejected","path":"webhooks/payloads/partners/rejected","children":[]},{"title":"Activated KYC Pending","path":"webhooks/payloads/partners/activated-kyc-pending","children":[]},{"title":"Funds On Hold","path":"webhooks/payloads/partners/funds-onhold","children":[]},{"title":"Funds Unhold","path":"webhooks/payloads/partners/funds-unhold","children":[]},{"title":"Instantly Activated","path":"webhooks/payloads/partners/instantly-activated","children":[]},{"title":"Payment Enabled","path":"webhooks/payloads/partners/payment-enabled","children":[]}],"layout":""}],"layout":""},{"title":"Route","path":"webhooks/payloads/route","children":[]},{"title":"Smart Collect","path":"webhooks/payloads/smart-collect","children":[]},{"title":"Payment Links","path":"webhooks/payloads/payment-links","children":[]},{"title":"RazorpayX","path":"webhooks/payloads/x","children":[]}],"layout":""},{"title":"FAQs","path":"webhooks/faqs","children":[]}]},{"title":"Security","children":[{"title":"About Razorpay Security","path":"security","children":[]},{"title":"Business Security Checklist","path":"security/checklist","children":[]},{"title":"Shared Responsibility Model","path":"security/shared-responsibility-model","children":[]},{"title":"IPs and Certificates","path":"security/whitelists","children":[]},{"title":"Security For Customers","path":"security/customers","children":[]}]}]},{"title":"Instant Refunds","hidden":true,"children":[{"title":"Instant Refunds","path":"api/instant-refunds","children":[],"layout":"api"}]},{"title":"Product Configuration APIs","hidden":true,"children":[]},{"title":"Products API","hidden":true,"children":[{"title":"Products API","path":"api/orders/products","children":[],"layout":"api"}]},{"title":"RazorpayX APIs - Skip Workflow","hidden":true,"children":[{"title":"RazorpayX APIs - Skip Workflow","path":"api/x/skip-workflow","children":[],"layout":"api"}]},{"title":"Security Risks - PCI DSS Non-Compliance","hidden":true,"children":[]},{"title":"Customer Payment History","hidden":true,"children":[]},{"title":"Form POST Payments","hidden":true,"children":[]},{"title":"Payment Downtime API","hidden":true,"children":[{"title":"Payment Downtime API","path":"api/payments/downtime-beta","children":[],"layout":"api"}]},{"title":"Recurring Payments API","hidden":true,"children":[{"title":"Recurring Payments","path":"api/payments/recurring-payments","children":[],"layout":"api"},{"title":"Postman Collection","path":"api/payments/recurring-payments/postman-collection","children":[],"layout":"api"},{"title":"Emandate","path":"","children":[{"title":"1. Create the Authorisation Transaction","path":"api/payments/recurring-payments/emandate/create-authorization-transaction","children":[],"layout":"api"},{"title":"2. Fetch and Manage Tokens","path":"api/payments/recurring-payments/emandate/tokens","children":[],"layout":"api"},{"title":"3. Create Subsequent Payments","path":"api/payments/recurring-payments/emandate/create-subsequent-payments","children":[],"layout":"api"}],"layout":""},{"title":"Cards","path":"","children":[{"title":"1. Create the Authorisation Transaction","path":"api/payments/recurring-payments/cards/create-authorization-transaction","children":[],"layout":"api"},{"title":"2. Fetch and Manage Tokens","path":"api/payments/recurring-payments/cards/tokens","children":[],"layout":"api"},{"title":"3. Create Subsequent Payments","path":"api/payments/recurring-payments/cards/create-subsequent-payments","children":[],"layout":"api"}],"layout":""},{"title":"Paper NACH","path":"","children":[{"title":"1. Create the Authorisation Transaction","path":"api/payments/recurring-payments/paper-nach/create-authorization-transaction","children":[],"layout":"api"},{"title":"2. Fetch and Manage Tokens","path":"api/payments/recurring-payments/paper-nach/tokens","children":[],"layout":"api"},{"title":"3. Create Subsequent Payments","path":"api/payments/recurring-payments/paper-nach/create-subsequent-payments","children":[],"layout":"api"}],"layout":""},{"title":"UPI","path":"","children":[{"title":"UPI","path":"","children":[{"title":"1. Create an Authorisation Transaction","path":"api/payments/recurring-payments/upi/create-authorization-transaction","children":[],"layout":"api"},{"title":"2. Fetch and Manage Tokens","path":"api/payments/recurring-payments/upi/tokens","children":[],"layout":"api"},{"title":"3. Create Subsequent Payments","path":"api/payments/recurring-payments/upi/create-subsequent-payments","children":[],"layout":"api"}],"layout":""},{"title":"UPI with TPV","path":"","children":[{"title":"1. Create the Authorization Transaction","path":"api/payments/recurring-payments/upi-tpv/create-authorization-transaction","children":[],"layout":"api"},{"title":"2. Fetch and Manage Tokens","path":"api/payments/recurring-payments/upi-tpv/tokens","children":[],"layout":"api"},{"title":"3. Create Subsequent Payments","path":"api/payments/recurring-payments/upi-tpv/create-subsequent-payments","children":[],"layout":"api"}],"layout":""}],"layout":""},{"title":"Registration and Charge First Payment Together","path":"","children":[{"title":"Emandate","path":"api/payments/recurring-payments/emandate/auto-debit","children":[],"layout":"api"},{"title":"Paper NACH","path":"api/payments/recurring-payments/paper-nach/auto-debit","children":[],"layout":"api"}],"layout":""},{"title":"Webhooks","path":"api/payments/recurring-payments/webhooks","children":[],"layout":"api"}]},{"title":"Card Fingerprints (or PAR) API","hidden":true,"children":[{"title":"Card Fingerprints (or PAR) API","path":"api/payments/cards/fingerprints","children":[],"layout":"api"}]},{"title":"Managing Reminders for Payment Links","hidden":true,"children":[]},{"title":"About Payment Links Customisation","hidden":true,"children":[]},{"title":"Account APIs [beta]","hidden":true,"children":[]},{"title":"Account APIs [beta]","hidden":true,"children":[]},{"title":"Subscriptions","hidden":true,"children":[]},{"title":"QR Codes (with Image Content)","hidden":true,"children":[]},{"title":"QR Codes GST APIs","hidden":true,"children":[{"title":"QR Codes GST APIs","path":"api/qr-codes/gst","children":[],"layout":"api"}]},{"title":"Additional Features","hidden":true,"children":[]},{"title":"Checkout Examples","hidden":true,"children":[]},{"title":"Partner Earnings","hidden":true,"children":[]},{"title":"About Platform Partners","hidden":true,"children":[{"title":"About Platform Partners","path":"partners/platform","children":[]},{"title":"Become a Platform Partner","path":"partners/platform/become-platform-partner","children":[]},{"title":"About OAuth","path":"","children":[{"title":"About Razorpay OAuth","path":"partners/platform/oauth","children":[]},{"title":"1. Build Integration","path":"partners/platform/oauth/integration-steps","children":[]},{"title":"2. Test Integration","path":"partners/platform/oauth/test-integration","children":[]},{"title":"3. Go-live Checklist","path":"partners/platform/oauth/go-live-checklist","children":[]},{"title":"Subscribe to Webhooks","path":"partners/platform/oauth/subscribe-to-webhooks","children":[]},{"title":"Revoke Access to Application","path":"partners/platform/oauth/revoke-access","children":[]},{"title":"Supported Products","path":"","children":[{"title":"Recurring Payments for Partners","path":"partners/platform/oauth/recurring-payments","children":[]},{"title":"Emandate","path":"","children":[{"title":"1. Emandate Registration","path":"partners/platform/oauth/recurring-payments/emandate/registration","children":[]},{"title":"2. Fetch and Manage Tokens","path":"partners/platform/oauth/recurring-payments/emandate/fetch-manage-tokens","children":[]},{"title":"3. Create Subsequent Payments","path":"partners/platform/oauth/recurring-payments/emandate/create-subsequent-payments","children":[]}],"layout":""},{"title":"Cards","path":"","children":[{"title":"1. Create Authorisation Transaction","path":"partners/platform/oauth/recurring-payments/cards/create-authorisation-transaction","children":[]},{"title":"2. Fetch and Manage Tokens","path":"partners/platform/oauth/recurring-payments/cards/fetch-manage-tokens","children":[]},{"title":"3. Create Subsequent Payments","path":"partners/platform/oauth/recurring-payments/cards/create-subsequent-payments","children":[]}],"layout":""},{"title":"UPI","path":"","children":[{"title":"1. Create Authorisation Transaction","path":"partners/platform/oauth/recurring-payments/upi/create-authorisation-transaction","children":[]},{"title":"2. Fetch and Manage Tokens","path":"partners/platform/oauth/recurring-payments/upi/fetch-manage-tokens","children":[]},{"title":"3. Create Subsequent Payments","path":"partners/platform/oauth/recurring-payments/upi/create-subsequent-payments","children":[]}],"layout":""},{"title":"UPI With TPV","path":"","children":[{"title":"1. Create Authorisation Transaction","path":"partners/platform/oauth/recurring-payments/upi-tpv/create-authorisation-transaction","children":[]},{"title":"2. Fetch and Manage Tokens","path":"partners/platform/oauth/recurring-payments/upi-tpv/fetch-manage-tokens","children":[]},{"title":"3. Create Subsequent Payments","path":"partners/platform/oauth/recurring-payments/upi-tpv/create-subsequent-payments","children":[]}],"layout":""}],"layout":""}],"layout":""}]},{"title":"Route for Partners","hidden":true,"children":[{"title":"Route","path":"partners/route","children":[]},{"title":"Linked Account APIs","path":"partners/route/linked-accounts","children":[]},{"title":"Transfers APIs","path":"partners/route/transfers","children":[]},{"title":"Settlement APIs","path":"partners/route/settlements","children":[]},{"title":"Refunds and Reversals APIs","path":"partners/route/refunds-reversals","children":[]}]},{"title":"Bulk Submerchant Upload","hidden":true,"children":[]},{"title":"Xpress Onboarding","hidden":true,"children":[{"title":"Xpress Onboarding","path":"partners/aggregators/xpress-onboarding","children":[]}]},{"title":"About Merchant Onboarding UI","hidden":true,"children":[{"title":"About Merchant Onboarding UI","path":"partners/aggregators/onboarding-ui","children":[]},{"title":"Integration Steps","path":"","children":[{"title":"1. Build Integration","path":"partners/aggregators/onboarding-ui/build-integration","children":[]},{"title":"2. Test Integration","path":"partners/aggregators/onboarding-ui/test-integration","children":[]}],"layout":""},{"title":"Onboarding Status","path":"partners/aggregators/onboarding-ui/status","children":[]}]},{"title":"About Recurring Payments for Partners","hidden":true,"children":[]},{"title":"Instantly Activate Sub-Merchant Accounts","hidden":true,"children":[]},{"title":"Become a Platform Partner","hidden":true,"children":[]},{"title":"New Sub-merchant Invite Flow","hidden":true,"children":[]},{"title":"Payment Link/Invoices Callback Support","hidden":true,"children":[]},{"title":"Razorpay Support Ticket API","hidden":true,"children":[]},{"title":"Microsoft .NET 3.5 Integration","hidden":true,"children":[]},{"title":"Dynamic Convenience Fees","hidden":true,"children":[{"title":"Dynamic Convenience Fees","path":"payments/dynamic-convenience-fees","children":[]},{"title":"API","path":"payments/dynamic-convenience-fees/api","children":[],"layout":"api"},{"title":"FAQs","path":"payments/dynamic-convenience-fees/faqs","children":[]}]},{"title":"Payment Methods for Merchant Categories","hidden":true,"children":[{"title":"Availability of Payment Methods as per Merchant Categories","path":"payments/merchant-categorisation","children":[]},{"title":"Financial Services","path":"","children":[{"title":"Financial Services Subcategories","path":"payments/merchant-categorisation/financial-services","children":[]},{"title":"Mutual Funds","path":"payments/merchant-categorisation/financial-services/mutual-funds","children":[]},{"title":"Lending","path":"payments/merchant-categorisation/financial-services/lending","children":[]},{"title":"Insurance","path":"payments/merchant-categorisation/financial-services/insurance","children":[]},{"title":"NBFC","path":"payments/merchant-categorisation/financial-services/nbfc","children":[]},{"title":"Cooperatives","path":"payments/merchant-categorisation/financial-services/cooperatives","children":[]},{"title":"Pension Fund","path":"payments/merchant-categorisation/financial-services/pension-fund","children":[]},{"title":"Forex","path":"payments/merchant-categorisation/financial-services/forex","children":[]},{"title":"Securities","path":"payments/merchant-categorisation/financial-services/securities","children":[]},{"title":"Commodities","path":"payments/merchant-categorisation/financial-services/commodities","children":[]},{"title":"Accounting and Taxes","path":"payments/merchant-categorisation/financial-services/accounting-taxes","children":[]},{"title":"Financial Advisory","path":"payments/merchant-categorisation/financial-services/financial-advisory","children":[]},{"title":"Crowdfunding Platform","path":"payments/merchant-categorisation/financial-services/crowdfunding-platform","children":[]},{"title":"Stock Broking and Trading","path":"payments/merchant-categorisation/financial-services/stock-broking","children":[]}],"layout":""},{"title":"Education","path":"","children":[{"title":"Education Subcategories","path":"payments/merchant-categorisation/education","children":[]},{"title":"College","path":"payments/merchant-categorisation/education/college","children":[]},{"title":"School","path":"payments/merchant-categorisation/education/school","children":[]},{"title":"University","path":"payments/merchant-categorisation/education/university","children":[]},{"title":"Professional Courses","path":"payments/merchant-categorisation/education/professional-courses","children":[]},{"title":"Distance Learning","path":"payments/merchant-categorisation/education/distance-learning","children":[]},{"title":"Coaching Institute","path":"payments/merchant-categorisation/education/coaching-institute","children":[]},{"title":"E-learning","path":"payments/merchant-categorisation/education/e-learning","children":[]},{"title":"Preschool and Day Care","path":"payments/merchant-categorisation/education/preschool-daycare","children":[]}],"layout":""},{"title":"Healthcare","path":"","children":[{"title":"Healthcare Subcategories","path":"payments/merchant-categorisation/healthcare","children":[]},{"title":"Clinic","path":"payments/merchant-categorisation/healthcare/clinic","children":[]},{"title":"Hospital","path":"payments/merchant-categorisation/healthcare/hospital","children":[]},{"title":"Lab","path":"payments/merchant-categorisation/healthcare/lab","children":[]},{"title":"Dietician","path":"payments/merchant-categorisation/healthcare/dietician","children":[]},{"title":"Gym and Fitness","path":"payments/merchant-categorisation/healthcare/gym-fitness","children":[]},{"title":"Health and Lifestyle Coaching","path":"payments/merchant-categorisation/healthcare/health-lifestyle-coaching","children":[]},{"title":"Health Products","path":"payments/merchant-categorisation/healthcare/health-products","children":[]},{"title":"Marketplace","path":"payments/merchant-categorisation/healthcare/marketplace","children":[]}],"layout":""},{"title":"Utilities","path":"","children":[{"title":"Utilities Subcategories","path":"payments/merchant-categorisation/utilities","children":[]},{"title":"Electricity","path":"payments/merchant-categorisation/utilities/electricity","children":[]},{"title":"Gas","path":"payments/merchant-categorisation/utilities/gas","children":[]},{"title":"Telecom Service Provider","path":"payments/merchant-categorisation/utilities/telecom-service","children":[]},{"title":"Water","path":"payments/merchant-categorisation/utilities/water","children":[]},{"title":"Cable Operator","path":"payments/merchant-categorisation/utilities/cable-operator","children":[]},{"title":"Broadband","path":"payments/merchant-categorisation/utilities/broadband","children":[]},{"title":"DTH","path":"payments/merchant-categorisation/utilities/dth","children":[]},{"title":"Internet Service Provider","path":"payments/merchant-categorisation/utilities/internet-service","children":[]},{"title":"Bill Payment and Recharge Aggregators","path":"payments/merchant-categorisation/utilities/bill-payment-recharge","children":[]}],"layout":""},{"title":"Government Bodies","path":"","children":[{"title":"Government Bodies Subcategories","path":"payments/merchant-categorisation/government-bodies","children":[]},{"title":"Central Department","path":"payments/merchant-categorisation/government-bodies/central-department","children":[]},{"title":"State Department","path":"payments/merchant-categorisation/government-bodies/state-department","children":[]}],"layout":""},{"title":"Logistics","path":"","children":[{"title":"Logistics Subcategories","path":"payments/merchant-categorisation/logistics","children":[]},{"title":"Freight Consolidation","path":"payments/merchant-categorisation/logistics/freight-consolidation","children":[]},{"title":"Courier Shipping","path":"payments/merchant-categorisation/logistics/courier-shipping","children":[]},{"title":"Public/Contract Warehousing","path":"payments/merchant-categorisation/logistics/public-contract-warehousing","children":[]},{"title":"Distribution Management","path":"payments/merchant-categorisation/logistics/distribution-management","children":[]},{"title":"End-to-End Logistics","path":"payments/merchant-categorisation/logistics/end-to-end-logistics","children":[]}],"layout":""},{"title":"Tours and Travels","path":"","children":[{"title":"Tours and Travels Subcategories","path":"payments/merchant-categorisation/tours-and-travels","children":[]},{"title":"Aviation","path":"payments/merchant-categorisation/tours-and-travels/aviation","children":[]},{"title":"Lodging and Accommodation","path":"payments/merchant-categorisation/tours-and-travels/lodging-accommodation","children":[]},{"title":"OTA","path":"payments/merchant-categorisation/tours-and-travels/ota","children":[]},{"title":"Tours and Travels Agency","path":"payments/merchant-categorisation/tours-and-travels/tours-travels-agency","children":[]}],"layout":""},{"title":"Transport","path":"","children":[{"title":"Transport Subcategories","path":"payments/merchant-categorisation/transport","children":[]},{"title":"Cab/Auto Hailing","path":"payments/merchant-categorisation/transport/cab-auto-hailing","children":[]},{"title":"Bus Ticketing","path":"payments/merchant-categorisation/transport/bus-ticketing","children":[]},{"title":"Train and Metro Ticketing","path":"payments/merchant-categorisation/transport/train-metro-ticketing","children":[]}],"layout":""},{"title":"Ecommerce","path":"","children":[{"title":"Ecommerce Subcategories","path":"payments/merchant-categorisation/ecommerce","children":[]},{"title":"Marketplace","path":"payments/merchant-categorisation/ecommerce/marketplace","children":[]},{"title":"Agricultural Products","path":"payments/merchant-categorisation/ecommerce/agricultural-products","children":[]},{"title":"Books and Publications","path":"payments/merchant-categorisation/ecommerce/books-publications","children":[]},{"title":"Electronics and Furniture","path":"payments/merchant-categorisation/ecommerce/electronics-furniture","children":[]},{"title":"Coupons and Deals","path":"payments/merchant-categorisation/ecommerce/coupons-deals","children":[]},{"title":"Product Rentals","path":"payments/merchant-categorisation/ecommerce/product-rentals","children":[]},{"title":"Fashion and Lifestyle","path":"payments/merchant-categorisation/ecommerce/fashion-lifestyle","children":[]},{"title":"Flowers and Gifts","path":"payments/merchant-categorisation/ecommerce/flowers-gifts","children":[]},{"title":"Grocery","path":"payments/merchant-categorisation/ecommerce/grocery","children":[]},{"title":"Baby Care and Toys","path":"payments/merchant-categorisation/ecommerce/baby-care-toys","children":[]},{"title":"Office Supplies","path":"payments/merchant-categorisation/ecommerce/office-supplies","children":[]},{"title":"Wholesale/Bulk Trade","path":"payments/merchant-categorisation/ecommerce/wholesale-bulk-trade","children":[]},{"title":"Religious Products","path":"payments/merchant-categorisation/ecommerce/religious-products","children":[]},{"title":"Pet Care and Supplies","path":"payments/merchant-categorisation/ecommerce/pet-care-supplies","children":[]},{"title":"Sports Goods","path":"payments/merchant-categorisation/ecommerce/sports-goods","children":[]},{"title":"Arts, Crafts and Collectibles","path":"payments/merchant-categorisation/ecommerce/arts-crafts-collectibles","children":[]},{"title":"Sexual Wellness Products","path":"payments/merchant-categorisation/ecommerce/sexual-wellness-products","children":[]},{"title":"Dropshipping","path":"payments/merchant-categorisation/ecommerce/dropshipping","children":[]}],"layout":""},{"title":"Food and Beverages","path":"","children":[{"title":"Food and Beverages Subcategories","path":"payments/merchant-categorisation/food-and-beverages","children":[]},{"title":"Online Food Ordering","path":"payments/merchant-categorisation/food-and-beverages/online-food-ordering","children":[]},{"title":"Restaurants","path":"payments/merchant-categorisation/food-and-beverages/restaurants","children":[]},{"title":"Food Courts/Corporate Cafeteria","path":"payments/merchant-categorisation/food-and-beverages/food-courts-cafeteria","children":[]},{"title":"Catering Services","path":"payments/merchant-categorisation/food-and-beverages/catering-services","children":[]},{"title":"Restaurant Search and Reservations","path":"payments/merchant-categorisation/food-and-beverages/restaurant-search-reservations","children":[]}],"layout":""},{"title":"IT and Software Services","path":"","children":[{"title":"IT and Software Services Subcategories","path":"payments/merchant-categorisation/it-and-software","children":[]},{"title":"Software as a Service (SaaS)","path":"payments/merchant-categorisation/it-and-software/saas","children":[]},{"title":"Platform as a Service (PaaS)","path":"payments/merchant-categorisation/it-and-software/paas","children":[]},{"title":"Infrastructure as a Service (IaaS)","path":"payments/merchant-categorisation/it-and-software/iaas","children":[]},{"title":"Consulting and Outsourcing","path":"payments/merchant-categorisation/it-and-software/consulting-outsourcing","children":[]},{"title":"Web Designing, Development and Hosting","path":"payments/merchant-categorisation/it-and-software/web-development","children":[]},{"title":"Technical Support","path":"payments/merchant-categorisation/it-and-software/technical-support","children":[]}],"layout":""},{"title":"Games","path":"","children":[{"title":"Games Subcategories","path":"payments/merchant-categorisation/games","children":[]},{"title":"Game Developer and Publisher","path":"payments/merchant-categorisation/games/game-developer-publisher","children":[]},{"title":"E-sports","path":"payments/merchant-categorisation/games/e-sports","children":[]},{"title":"Fantasy Sports","path":"payments/merchant-categorisation/games/fantasy-sports","children":[]},{"title":"Game Distribution and Marketplace","path":"payments/merchant-categorisation/games/game-distributor-marketplace","children":[]}],"layout":""},{"title":"Media and Entertainment","path":"","children":[{"title":"Media and Entertainment Subcategories","path":"payments/merchant-categorisation/media-and-entertainment","children":[]},{"title":"Video on Demand","path":"payments/merchant-categorisation/media-and-entertainment/video-on-demand","children":[]},{"title":"Music Streaming Services","path":"payments/merchant-categorisation/media-and-entertainment/music-streaming-services","children":[]},{"title":"Multiplexes","path":"payments/merchant-categorisation/media-and-entertainment/multiplexes","children":[]},{"title":"Content and Publishing","path":"payments/merchant-categorisation/media-and-entertainment/content-publishing","children":[]},{"title":"Events and Movie Ticketing","path":"payments/merchant-categorisation/media-and-entertainment/events-movie-ticketing","children":[]},{"title":"News","path":"payments/merchant-categorisation/media-and-entertainment/news","children":[]}],"layout":""},{"title":"Services","path":"","children":[{"title":"Services Subcategories","path":"payments/merchant-categorisation/services","children":[]},{"title":"Repair and Cleaning Services","path":"payments/merchant-categorisation/services/repair-cleaning-services","children":[]},{"title":"Interior Designing and Architect","path":"payments/merchant-categorisation/services/interior-designing-architect","children":[]},{"title":"Movers and Packers","path":"payments/merchant-categorisation/services/movers-packers","children":[]},{"title":"Legal Services","path":"payments/merchant-categorisation/services/legal-services","children":[]},{"title":"Event Planning Services","path":"payments/merchant-categorisation/services/event-planning-services","children":[]},{"title":"Service Centre","path":"payments/merchant-categorisation/services/service-centre","children":[]},{"title":"Consulting Services","path":"payments/merchant-categorisation/services/consulting-services","children":[]},{"title":"Ad and Marketing Agencies","path":"payments/merchant-categorisation/services/ad-marketing-agencies","children":[]},{"title":"Services Classifieds","path":"payments/merchant-categorisation/services/services-classifieds","children":[]}],"layout":""},{"title":"Housing and Real Estate","path":"","children":[{"title":"Housing and Real Estate Subcategories","path":"payments/merchant-categorisation/housing-real-estate","children":[]},{"title":"Developer","path":"payments/merchant-categorisation/housing-real-estate/developer","children":[]},{"title":"Facility Management Company","path":"payments/merchant-categorisation/housing-real-estate/facility-management-company","children":[]},{"title":"RWA","path":"payments/merchant-categorisation/housing-real-estate/rwa","children":[]},{"title":"Co-working Spaces","path":"payments/merchant-categorisation/housing-real-estate/co-working-spaces","children":[]},{"title":"Real Estate Classifieds","path":"payments/merchant-categorisation/housing-real-estate/real-estate-classifieds","children":[]},{"title":"Home and Office Rentals","path":"payments/merchant-categorisation/housing-real-estate/home-office-rentals","children":[]}],"layout":""},{"title":"Not-For-Profit","path":"","children":[{"title":"Not-for-Profit Subcategories","path":"payments/merchant-categorisation/not-for-profit","children":[]},{"title":"Charity","path":"payments/merchant-categorisation/not-for-profit/charity","children":[]},{"title":"Educational","path":"payments/merchant-categorisation/not-for-profit/educational","children":[]},{"title":"Religious","path":"payments/merchant-categorisation/not-for-profit/religious","children":[]},{"title":"Personal","path":"payments/merchant-categorisation/not-for-profit/personal","children":[]}],"layout":""},{"title":"Social","path":"","children":[{"title":"Social Subcategories","path":"payments/merchant-categorisation/social","children":[]},{"title":"Dating and Matrimony Platforms","path":"payments/merchant-categorisation/social/dating-matrimony-platforms","children":[]},{"title":"Social Network","path":"payments/merchant-categorisation/social/social-network","children":[]},{"title":"Messaging and Communication","path":"payments/merchant-categorisation/social/messaging-communication","children":[]},{"title":"Professional Network","path":"payments/merchant-categorisation/social/professional-network","children":[]},{"title":"Local/Neighbourhood Network","path":"payments/merchant-categorisation/social/local-neighbourhood-network","children":[]}],"layout":""},{"title":"Others","path":"payments/merchant-categorisation/others","children":[]}]},{"title":"Razorpay Referral Program","hidden":true,"children":[{"title":"Razorpay Referral Program","path":"payments/referral-program","children":[]}]},{"title":"Recurring Payments","hidden":true,"children":[{"title":"Recurring Payments","path":"payments/recurring-payments","children":[]},{"title":"Emandate","path":"","children":[{"title":"Integrate Recurring Payments","path":"payments/recurring-payments/emandate/integrate","children":[]},{"title":"Charge Customers During Registration","path":"payments/recurring-payments/emandate/charge-customer-during-registration","children":[]},{"title":"Supported Banks","path":"payments/recurring-payments/emandate/supported-banks","children":[]},{"title":"APIs","path":"payments/recurring-payments/emandate/apis","children":[]},{"title":"FAQs","path":"payments/recurring-payments/emandate/faqs","children":[]},{"title":"Handle Errors","path":"payments/recurring-payments/emandate/errors","children":[]}],"layout":""},{"title":"Cards","path":"","children":[{"title":"Integrate Recurring Payments","path":"payments/recurring-payments/cards/integrate","children":[]},{"title":"Supported Banks","path":"payments/recurring-payments/cards/supported-banks","children":[]},{"title":"APIs","path":"payments/recurring-payments/cards/apis","children":[]},{"title":"FAQs","path":"payments/recurring-payments/cards/faqs","children":[]}],"layout":""},{"title":"Paper NACH","path":"","children":[{"title":"Integrate Recurring Payments","path":"payments/recurring-payments/paper-nach/integrate","children":[]},{"title":"APIs","path":"payments/recurring-payments/paper-nach/apis","children":[]},{"title":"FAQs","path":"payments/recurring-payments/paper-nach/faqs","children":[]}],"layout":""},{"title":"UPI","path":"","children":[{"title":"Integrate Recurring Payments","path":"payments/recurring-payments/upi/integrate","children":[]},{"title":"Supported Banks","path":"payments/recurring-payments/upi/supported-banks","children":[]},{"title":"QR Codes","path":"payments/recurring-payments/upi/qr-codes","children":[]},{"title":"APIs","path":"payments/recurring-payments/upi/apis","children":[]},{"title":"FAQs","path":"payments/recurring-payments/upi/faqs","children":[]}],"layout":""},{"title":"Dashboard","path":"","children":[{"title":"Create a Recurring Payment","path":"payments/recurring-payments/create","children":[]},{"title":"Paper NACH Form","path":"payments/recurring-payments/upload-paper-nach-form","children":[]},{"title":"Batch Operations","path":"payments/recurring-payments/batch-operations","children":[]}],"layout":""},{"title":"Webhooks","path":"payments/recurring-payments/subscribe-to-webhooks","children":[]},{"title":"Glossary","path":"payments/recurring-payments/glossary","children":[]}]},{"title":"Razorpay White Label Wallet","hidden":true,"children":[{"title":"Razorpay White Label Wallet","path":"payments/wallet","children":[]},{"title":"Wallet Operations","path":"payments/wallet/wallet-operations","children":[]},{"title":"API Reference","path":"payments/wallet/api-reference","children":[]}]},{"title":"Add Buyer's Address","hidden":true,"children":[]},{"title":"Upload Invoices","hidden":true,"children":[]},{"title":"Balances","hidden":true,"children":[{"title":"Balances","path":"payments/dashboard/my-account/balances-beta","children":[]}]},{"title":"Credits","hidden":true,"children":[{"title":"Credits","path":"payments/dashboard/my-account/credits-beta","children":[]}]},{"title":"Collect Convenience Fees from Customers","hidden":true,"children":[{"title":"Collect Convenience Fees from Customers","path":"payments/dashboard/account-settings/configuration/convenience-fees","children":[]}]},{"title":"Negative Balance for eMandate Registrations","hidden":true,"children":[]},{"title":"Negative Balance for Refunds and Route","hidden":true,"children":[]},{"title":"Customer Fund Account APIs","hidden":true,"children":[]},{"title":"Disputes","hidden":true,"children":[{"title":"Disputes","path":"payments/disputes/presentments","children":[]}]},{"title":"L1 & L2 videos","hidden":true,"children":[]},{"title":"Handle Payment Exceptions with Rainy Day Kit","hidden":true,"children":[{"title":"Rainy Day Kit","path":"payments/payment-gateway/rainy-day","children":[]},{"title":"Payment Capture Settings","path":"","children":[{"title":"About Payment Capture Settings","path":"payments/payment-gateway/rainy-day/capture-settings","children":[]},{"title":"API","path":"payments/payment-gateway/rainy-day/capture-settings/api","children":[]}],"layout":""},{"title":"Payment Downtime Notifications","path":"","children":[{"title":"About Payment Downtime API","path":"payments/payment-gateway/rainy-day/downtime","children":[]}],"layout":""},{"title":"Payment Errors Codes","path":"","children":[{"title":"About Errors","path":"payments/payment-gateway/rainy-day/errors","children":[]},{"title":"Error Codes","path":"payments/payment-gateway/rainy-day/errors/error-codes","children":[]},{"title":"Error Reasons","path":"payments/payment-gateway/rainy-day/errors/error-reasons","children":[]},{"title":"Payment Method Error Parameters","path":"payments/payment-gateway/rainy-day/errors/payment-error-parameters","children":[]}],"layout":""}]},{"title":"Zoho Integration","hidden":true,"children":[]},{"title":"Server-to-Server Integration","hidden":true,"children":[{"title":"Server-to-Server Integration","path":"payments/payment-gateway/s2s-integration","children":[]},{"title":"Integration Versions","path":"","children":[{"title":"S2S JSON V2 (Latest)","path":"","children":[{"title":"About Server-to-Server JSON V2 Integration","path":"payments/payment-gateway/s2s-integration/json/v2","children":[]},{"title":"1. Build Integration","path":"","children":[{"title":"Netbanking","path":"payments/payment-gateway/s2s-integration/json/v2/build-integration/netbanking","children":[]},{"title":"Cards","path":"","children":[{"title":"New Integration","path":"payments/payment-gateway/s2s-integration/json/v2/build-integration/cards","children":[]},{"title":"Existing Integration (Migrate to 3DS2)","path":"payments/payment-gateway/s2s-integration/json/v2/build-integration/cards/migrate-3ds2.0","children":[]}],"layout":""},{"title":"UPI","path":"payments/payment-gateway/s2s-integration/json/v2/build-integration/upi","children":[]}],"layout":""},{"title":"2. Test Integration","path":"payments/payment-gateway/s2s-integration/json/v2/test-integration","children":[]},{"title":"3. Go-live Checklist","path":"payments/payment-gateway/s2s-integration/json/v2/go-live-checklist","children":[]}],"layout":""},{"title":"S2S JSON V1","path":"","children":[{"title":"About Server-to-Server JSON V1 Integration","path":"payments/payment-gateway/s2s-integration/json/v1","children":[]},{"title":"1. Build Integration","path":"","children":[{"title":"UPI","path":"payments/payment-gateway/s2s-integration/json/v1/build-integration/upi","children":[]},{"title":"Cards","path":"","children":[{"title":"New Integration","path":"payments/payment-gateway/s2s-integration/json/v1/build-integration/cards","children":[]},{"title":"Existing Integration (Migrate to 3DS2)","path":"payments/payment-gateway/s2s-integration/json/v1/build-integration/cards/migrate-3ds2.0","children":[]}],"layout":""}],"layout":""},{"title":"2. Test Integration","path":"payments/payment-gateway/s2s-integration/json/v1/test-integration","children":[]},{"title":"3. Go-live Checklist","path":"payments/payment-gateway/s2s-integration/json/v1/go-live-checklist","children":[]}],"layout":""},{"title":"S2S Redirect","path":"","children":[{"title":"About Server-to-Server Redirect Integration","path":"payments/payment-gateway/s2s-integration/redirect","children":[]},{"title":"Build Integration","path":"","children":[{"title":"Cards","path":"","children":[{"title":"New Integration","path":"payments/payment-gateway/s2s-integration/redirect/build-integration/cards","children":[]},{"title":"Existing Integration (Migrate to 3DS2)","path":"payments/payment-gateway/s2s-integration/redirect/build-integration/cards/migrate-3ds2.0","children":[]}],"layout":""},{"title":"Other Payment Methods","path":"payments/payment-gateway/s2s-integration/redirect/build-integration","children":[]}],"layout":""},{"title":"2. Test Integration","path":"payments/payment-gateway/s2s-integration/redirect/test-integration","children":[]},{"title":"3. Go-live Checklist","path":"payments/payment-gateway/s2s-integration/redirect/go-live-checklist","children":[]}],"layout":""}],"layout":""},{"title":"Best Practices","path":"payments/payment-gateway/s2s-integration/best-practices","children":[]},{"title":"Payment Methods","path":"","children":[{"title":"Payment Methods","path":"payments/payment-gateway/s2s-integration/payment-methods","children":[]},{"title":"CVV less Flow for Card Payments","path":"payments/payment-gateway/s2s-integration/payment-methods/cvv-less-flow","children":[]},{"title":"Methods API","path":"payments/payment-gateway/s2s-integration/payment-methods/methods-api","children":[],"layout":"product"},{"title":"PayPal","path":"payments/payment-gateway/s2s-integration/payment-methods/paypal","children":[]},{"title":"3DS2 Protocol for Card Payments","path":"payments/payment-gateway/s2s-integration/payment-methods/cards/3ds2.0","children":[]},{"title":"UPI","path":"","children":[{"title":"About UPI Payments","path":"payments/payment-gateway/s2s-integration/payment-methods/upi","children":[]},{"title":"Collect Flow","path":"payments/payment-gateway/s2s-integration/payment-methods/upi/collect","children":[]},{"title":"Intent Flow","path":"payments/payment-gateway/s2s-integration/payment-methods/upi/intent","children":[]},{"title":"Saved VPA","path":"","children":[{"title":"About Saved VPA in Server-to-Server Integration","path":"payments/payment-gateway/s2s-integration/payment-methods/upi/saved-vpa","children":[]},{"title":"Build Integration","path":"payments/payment-gateway/s2s-integration/payment-methods/upi/saved-vpa/build-integration","children":[]}],"layout":""}],"layout":""}],"layout":""},{"title":"Features","path":"","children":[{"title":"Address Verification System","path":"payments/payment-gateway/s2s-integration/features/address-verification-system","children":[]}],"layout":""}]},{"title":"Eligibility Check API","hidden":true,"children":[{"title":"Eligibility Check API","path":"payments/payment-gateway/affordability/eligibility-check","children":[]},{"title":"Configure Affordability Methods","path":"payments/payment-gateway/affordability/eligibility-check/configurations","children":[]}]},{"title":"Integrating Offers with Custom Checkout","hidden":true,"children":[]},{"title":"Integrating Offers in Server-to-Server (S2S)","hidden":true,"children":[]},{"title":"Integrate Payment Methods in Custom Checkout","hidden":true,"children":[]},{"title":"Integrate Affordability Widget With Shopify","hidden":true,"children":[]},{"title":"Integrate With Android Custom SDK","hidden":true,"children":[{"title":"Integrate With Android Custom SDK","path":"payments/payment-gateway/android-integration/custom","children":[]},{"title":"1. Build Integration","path":"payments/payment-gateway/android-integration/custom/build-integration","children":[]},{"title":"2. Test Integration","path":"payments/payment-gateway/android-integration/custom/test-integration","children":[]},{"title":"3. Go-live Checklist","path":"payments/payment-gateway/android-integration/custom/go-live-checklist","children":[]},{"title":"Payment Methods","path":"payments/payment-gateway/android-integration/custom/payment-methods","children":[]},{"title":"Turbo UPI","path":"","children":[{"title":"About Turbo UPI","path":"payments/payment-gateway/android-integration/custom/payment-methods/turbo-upi","children":[]},{"title":"Integrate Turbo UPI UI","path":"payments/payment-gateway/android-integration/custom/payment-methods/turbo-upi/integration-ui","children":[]},{"title":"Integrate Turbo UPI Headless","path":"payments/payment-gateway/android-integration/custom/payment-methods/turbo-upi/integration-noui","children":[]}],"layout":""},{"title":"Additional Support for Payment Methods","path":"payments/payment-gateway/android-integration/custom/additional-features","children":[]},{"title":"Native OTP Integration","path":"","children":[{"title":"1. Native OTP Integration","path":"payments/payment-gateway/android-integration/custom/native-otp-integration","children":[]},{"title":"2. Test Native OTP Integration","path":"payments/payment-gateway/android-integration/custom/test-native-otp-integration","children":[]}],"layout":""},{"title":"Override Minimum SDK Version","path":"payments/payment-gateway/android-integration/custom/override-minimum-sdk","children":[]},{"title":"Troubleshooting & FAQs","path":"payments/payment-gateway/android-integration/custom/troubleshooting-faqs","children":[]},{"title":"Google Play Console - Data Safety","path":"payments/payment-gateway/android-integration/custom/google-data-safety","children":[]}]},{"title":"Magic Plugin for Android Custom UI SDK","hidden":true,"children":[{"title":"Magic Plugin for Android Custom UI SDK","path":"payments/payment-gateway/android-integration/magic","children":[]},{"title":"Magic Plugin Integration Guide","path":"payments/payment-gateway/android-integration/magic/add-sdk","children":[]},{"title":"Custom Magic Layout","path":"payments/payment-gateway/android-integration/magic/custom-layout","children":[]}]},{"title":"Integrate With iOS Custom SDK","hidden":true,"children":[{"title":"Integrate with iOS Custom SDK","path":"payments/payment-gateway/ios-integration/custom","children":[]},{"title":"1. Build Integration","path":"payments/payment-gateway/ios-integration/custom/build-integration","children":[]},{"title":"2. Test Integration","path":"payments/payment-gateway/ios-integration/custom/test-integration","children":[]},{"title":"3. Go-live Checklist","path":"payments/payment-gateway/ios-integration/custom/go-live-checklist","children":[]},{"title":"Additional Support for Payment Methods","path":"payments/payment-gateway/ios-integration/custom/payment-methods","children":[]},{"title":"Turbo UPI","path":"","children":[{"title":"About Turbo UPI","path":"payments/payment-gateway/ios-integration/custom/payment-methods/turbo-upi","children":[]},{"title":"Integrate Turbo UPI UI","path":"payments/payment-gateway/ios-integration/custom/payment-methods/turbo-upi/integrate-ui","children":[]},{"title":"Integrate Turbo UPI Headless","path":"payments/payment-gateway/ios-integration/custom/payment-methods/turbo-upi/integrate-noui","children":[]}],"layout":""},{"title":"Native OTP Integration","path":"","children":[{"title":"1. Native OTP Integration","path":"payments/payment-gateway/ios-integration/custom/native-otp","children":[]},{"title":"2. Test Native OTP Integration","path":"payments/payment-gateway/ios-integration/custom/test-native-otp","children":[]}],"layout":""},{"title":"Additional Configurations","path":"payments/payment-gateway/ios-integration/custom/configurations","children":[]},{"title":"Troubleshooting & FAQs","path":"payments/payment-gateway/ios-integration/custom/troubleshooting-faqs","children":[]}]},{"title":"Web Integration - Razorpay Custom Checkout","hidden":true,"children":[{"title":"Integrate with Web Custom SDK","path":"payments/payment-gateway/web-integration/custom","children":[]},{"title":"1. Build Integration","path":"payments/payment-gateway/web-integration/custom/build-integration","children":[]},{"title":"2. Test Integration","path":"payments/payment-gateway/web-integration/custom/test-integration","children":[]},{"title":"3. Go-live Checklist","path":"payments/payment-gateway/web-integration/custom/go-live-checklist","children":[]},{"title":"Best Practices","path":"payments/payment-gateway/web-integration/custom/best-practices","children":[]},{"title":"Troubleshooting & FAQs","path":"payments/payment-gateway/web-integration/custom/troubleshooting-faqs","children":[]},{"title":"Additional Options","path":"","children":[{"title":"Additional Support For Payment Methods","path":"payments/payment-gateway/web-integration/custom/payment-methods","children":[]},{"title":"Custom Fields","path":"payments/payment-gateway/web-integration/custom/input-restriction","children":[]}],"layout":""},{"title":"Features","path":"","children":[{"title":"Native OTP","path":"payments/payment-gateway/web-integration/custom/features/native-otp","children":[]},{"title":"Saved Cards","path":"","children":[{"title":"Save Customer Card Details as Network Tokens","path":"payments/payment-gateway/web-integration/custom/features/saved-cards","children":[]},{"title":"CVV less Flow for Card Payments","path":"payments/payment-gateway/web-integration/custom/features/cvv-less-flow","children":[]},{"title":"Integration Steps","path":"","children":[{"title":"Business Seeks Customer Consent, Saves Card Details with Razorpay","path":"payments/payment-gateway/web-integration/custom/features/saved-cards/scenario-1","children":[]},{"title":"Razorpay Seeks Customer Consent on Behalf of Business","path":"payments/payment-gateway/web-integration/custom/features/saved-cards/scenario-2","children":[]},{"title":"Business Seeks Consent from Some Customers Only","path":"payments/payment-gateway/web-integration/custom/features/saved-cards/scenario-3","children":[]}],"layout":""}],"layout":""},{"title":"Validate VPA","path":"payments/payment-gateway/web-integration/custom/features/validate-vpa","children":[]},{"title":"Saved VPA","path":"payments/payment-gateway/web-integration/custom/features/saved-vpa","children":[]},{"title":"EMI Plans","path":"payments/payment-gateway/web-integration/custom/features/emi-plans","children":[]},{"title":"Create Async Payment","path":"payments/payment-gateway/web-integration/custom/features/async-payments","children":[]},{"title":"Bring a Pop-up to the Front","path":"payments/payment-gateway/web-integration/custom/features/pop-up","children":[]},{"title":"Check CRED Eligibility","path":"payments/payment-gateway/web-integration/custom/features/check-cred-eligibility","children":[]}],"layout":""}]},{"title":"Integrate with Hosted Checkout","hidden":true,"children":[]},{"title":"Standard Web Integration - Configurability of Payment Methods","hidden":true,"children":[{"title":"Standard Web Integration - Configurability of Payment Methods","path":"payments/payment-gateway/web-integration/standard/configure-restrict-payment-methods","children":[]},{"title":"Sample Codes","path":"payments/payment-gateway/web-integration/standard/configure-restrict-payment-methods/sample-code","children":[]}]},{"title":"Integrate With React Native Custom SDK","hidden":true,"children":[{"title":"Integrate with React Native Custom SDK","path":"payments/payment-gateway/react-native-integration/custom","children":[]},{"title":"1. Build Integration","path":"payments/payment-gateway/react-native-integration/custom/build-integration","children":[]},{"title":"2. Test Integration","path":"payments/payment-gateway/react-native-integration/custom/test-integration","children":[]},{"title":"3. Go-live Checklist","path":"payments/payment-gateway/react-native-integration/custom/go-live-checklist","children":[]},{"title":"Additional Support for Payment Methods","path":"payments/payment-gateway/react-native-integration/custom/additional-features","children":[]},{"title":"Troubleshooting & FAQs","path":"payments/payment-gateway/react-native-integration/custom/troubleshooting-faqs","children":[]}]},{"title":"Integrate With Flutter Custom SDK","hidden":true,"children":[{"title":"Integrate with Flutter Custom SDK","path":"payments/payment-gateway/flutter-integration/custom","children":[]},{"title":"1. Build Integration","path":"payments/payment-gateway/flutter-integration/custom/build-integration","children":[]},{"title":"2. Test Integration","path":"payments/payment-gateway/flutter-integration/custom/test-integration","children":[]},{"title":"3. Go-live Checklist","path":"payments/payment-gateway/flutter-integration/custom/go-live-checklist","children":[]},{"title":"Additional Options","path":"","children":[{"title":"Payment Methods","path":"payments/payment-gateway/flutter-integration/custom/payment-methods","children":[]},{"title":"Package Methods","path":"payments/payment-gateway/flutter-integration/custom/methods","children":[]}],"layout":""},{"title":"Troubleshooting & FAQs","path":"payments/payment-gateway/flutter-integration/custom/troubleshooting-faqs","children":[]}]},{"title":"Magento 2.x Extension","hidden":true,"children":[]},{"title":"Payment Failure Analysis","hidden":true,"children":[{"title":"Payment Failure Analysis","path":"payments/payments/failure-analysis","children":[]}]},{"title":"Configure Payment Capture Settings using Orders API","hidden":true,"children":[{"title":"Configure Payment Capture Settings using Orders API","path":"payments/payments/capture-settings/api","children":[]}]},{"title":"API Contract Migration","hidden":true,"children":[{"title":"API Contract Migration","path":"payments/payment-links/announcements","children":[]},{"title":"Increase Order Conversion Rate with Retry Links","path":"payments/payment-links/announcements/retry-link","children":[]}]},{"title":"BharatQR","hidden":true,"children":[{"title":"BharatQR","path":"payments/payment-methods/bharatqr","children":[]},{"title":"API Reference","path":"payments/payment-methods/bharatqr/api","children":[]},{"title":"Additional Operations","path":"payments/payment-methods/bharatqr/additional-operations","children":[]},{"title":"Notifications","path":"payments/payment-methods/bharatqr/notification","children":[]},{"title":"Statuses","path":"payments/payment-methods/bharatqr/status","children":[]},{"title":"Testing","path":"payments/payment-methods/bharatqr/testing","children":[]},{"title":"Frequently Asked Questions","path":"payments/payment-methods/bharatqr/faqs","children":[]}]},{"title":"eCOD","hidden":true,"children":[{"title":"eCOD","path":"payments/payment-methods/ecod","children":[]},{"title":"Integrate eCOD","path":"payments/payment-methods/ecod/integration","children":[]}]},{"title":"About SWIFT Transfers","hidden":true,"children":[{"title":"About SWIFT Transfers","path":"payments/payment-methods/swift-bank-transfer","children":[]}]},{"title":"International Payments - POLi","hidden":true,"children":[{"title":"International Payments - POLi","path":"payments/payment-methods/poli","children":[]},{"title":"Custom Integration","path":"payments/payment-methods/poli/custom-integration","children":[]},{"title":"S2S Integration","path":"payments/payment-methods/poli/s2s-integration","children":[]}]},{"title":"International Payments - Sofort","hidden":true,"children":[{"title":"International Payments - Sofort","path":"payments/payment-methods/sofort","children":[]},{"title":"Custom Integration","path":"payments/payment-methods/sofort/custom-integration","children":[]},{"title":"S2S Integration","path":"payments/payment-methods/sofort/s2s-integration","children":[]}]},{"title":"International Payments - Trustly","hidden":true,"children":[{"title":"International Payments - Trustly","path":"payments/payment-methods/trustly","children":[]},{"title":"Custom Integration","path":"payments/payment-methods/trustly/custom-integration","children":[]},{"title":"S2S Integration","path":"payments/payment-methods/trustly/s2s-integration","children":[]}]},{"title":"UPI QR Code","hidden":true,"children":[{"title":"UPI QR Code","path":"payments/payment-methods/upi-qr","children":[]},{"title":"API Integration","path":"payments/payment-methods/upi-qr/api","children":[],"layout":"api"},{"title":"Webhook Notifications","path":"payments/payment-methods/upi-qr/webhooks","children":[]},{"title":"FAQs","path":"payments/payment-methods/upi-qr/faqs","children":[]}]},{"title":"International Payments - Giropay","hidden":true,"children":[{"title":"International Payments - Giropay","path":"payments/payment-methods/giropay","children":[]},{"title":"Custom Integration","path":"payments/payment-methods/giropay/custom-integration","children":[]},{"title":"S2S Integration","path":"payments/payment-methods/giropay/s2s-integration","children":[]}]},{"title":"Accept International Payments Using Local Currency Bank Transfer","hidden":true,"children":[{"title":"Accept International Payments Using Local Currency Bank Transfer","path":"payments/payment-methods/local-currency-bank-transfer","children":[]}]},{"title":"Accept Payments using CRED Pay","hidden":true,"children":[{"title":"Accept Payments using CRED Pay","path":"payments/payment-methods/apps/cred","children":[]},{"title":"Standard Integration","path":"","children":[{"title":"About Accepting Payments using CRED Pay on Standard Checkout","path":"payments/payment-methods/apps/cred/standard-integration","children":[]},{"title":"Display Cred on Checkout","path":"payments/payment-methods/apps/cred/standard-integration/checkout-configuration","children":[]}],"layout":""},{"title":"Custom Integration","path":"payments/payment-methods/apps/cred/custom-integration","children":[]},{"title":"S2S Integration","path":"payments/payment-methods/apps/cred/s2s-integration","children":[]},{"title":"Refunds","path":"payments/payment-methods/apps/cred/refunds","children":[]},{"title":"Pricing","path":"payments/payment-methods/apps/cred/pricing","children":[]}]},{"title":"Pay with Reward Points","hidden":true,"children":[{"title":"Pay with Reward Points","path":"payments/payment-methods/apps/reward-points","children":[]},{"title":"Custom Integration","path":"payments/payment-methods/apps/reward-points/custom-integration","children":[]},{"title":"S2S Integration","path":"","children":[{"title":"JSON API","path":"payments/payment-methods/apps/reward-points/s2s-integration/json","children":[]},{"title":"Redirect API","path":"payments/payment-methods/apps/reward-points/s2s-integration/redirect","children":[]}],"layout":""},{"title":"FAQs","path":"payments/payment-methods/apps/reward-points/faqs","children":[]}]},{"title":"Bank Transfer on Custom Checkout","hidden":true,"children":[{"title":"Bank Transfer on Custom Checkout","path":"payments/payment-methods/bank-transfer/custom-integration","children":[]}]},{"title":"Corporate Card Payments","hidden":true,"children":[]},{"title":"Dynamic Currency Conversion","hidden":true,"children":[{"title":"Dynamic Currency Conversion","path":"payments/payment-methods/cards/dynamic-currency-conversion","children":[]},{"title":"Custom Checkout Integration","path":"payments/payment-methods/cards/dynamic-currency-conversion/custom-integration","children":[]},{"title":"S2S Integration","path":"payments/payment-methods/cards/dynamic-currency-conversion/s2s-integration","children":[]}]},{"title":"Tokens (Private)","hidden":true,"children":[]},{"title":"Tokens (Public)","hidden":true,"children":[]},{"title":"Google Pay Card Payments","hidden":true,"children":[{"title":"Google Pay Card Payments","path":"payments/payment-methods/cards/google-pay","children":[]},{"title":"Android Integrations","path":"","children":[{"title":"Android Standard Checkout","path":"payments/payment-methods/cards/google-pay/standard-integration","children":[]},{"title":"Android Custom Checkout","path":"payments/payment-methods/cards/google-pay/custom-integration","children":[]}],"layout":""},{"title":"S2S Integrations","path":"","children":[{"title":"JSON API","path":"payments/payment-methods/cards/google-pay/s2s-integration/json","children":[]},{"title":"Redirect API","path":"payments/payment-methods/cards/google-pay/s2s-integration/redirect","children":[]}],"layout":""},{"title":"FAQs","path":"payments/payment-methods/cards/google-pay/faqs","children":[]}]},{"title":"Visa Safe Click for Payments via Juspay","hidden":true,"children":[]},{"title":"Authentication Type for Cards - Native OTP","hidden":true,"children":[{"title":"Authentication Type for Cards - Native OTP","path":"payments/payment-methods/cards/authentication/native-otp","children":[]}]},{"title":"TokenHQ - Issuer Tokenisation","hidden":true,"children":[]},{"title":"TokenHQ - Business as Token Requestor","hidden":true,"children":[{"title":"TokenHQ - Business as Token Requestor","path":"payments/payment-methods/cards/token-hq/merchant-requestor","children":[]},{"title":"APIs","path":"","children":[{"title":"Token Lifecycle","path":"payments/payment-methods/cards/token-hq/merchant-requestor/token-lifecycle","children":[]},{"title":"Tokenisation APIs","path":"payments/payment-methods/cards/token-hq/merchant-requestor/apis","children":[],"layout":"api"},{"title":"Token IIN API","path":"payments/payment-methods/cards/token-hq/merchant-requestor/iin-validation","children":[],"layout":"api"}],"layout":""},{"title":"Webhooks","path":"payments/payment-methods/cards/token-hq/merchant-requestor/webhooks","children":[],"layout":"api"},{"title":"Additional Information","path":"payments/payment-methods/cards/token-hq/merchant-requestor/additional-information","children":[]}]},{"title":"Tokenise Cards when Razorpay is Token Requestor","hidden":true,"children":[{"title":"Tokenise Cards when Razorpay is Token Requestor","path":"payments/payment-methods/cards/token-hq/razorpay-requestor","children":[]},{"title":"APIs","path":"","children":[{"title":"Token Lifecycle","path":"payments/payment-methods/cards/token-hq/razorpay-requestor/token-lifecycle","children":[]},{"title":"Tokenisation APIs","path":"payments/payment-methods/cards/token-hq/razorpay-requestor/apis","children":[],"layout":"api"},{"title":"IIN/BIN Validations on Tokens","path":"payments/payment-methods/cards/token-hq/razorpay-requestor/iin-validation","children":[],"layout":"api"}],"layout":""},{"title":"CVV-less Flow","path":"payments/payment-methods/cards/token-hq/razorpay-requestor/cvv-less-flow","children":[]},{"title":"Tokenisation Webhooks","path":"payments/payment-methods/cards/token-hq/razorpay-requestor/webhooks","children":[],"layout":"api"},{"title":"Additional Information","path":"payments/payment-methods/cards/token-hq/razorpay-requestor/additional-information","children":[]}]},{"title":"TokenHQ - Business as Token Requestor","hidden":true,"children":[{"title":"TokenHQ - Business as Token Requestor","path":"payments/payment-methods/cards/token-hq/merchant-requestor-with-network-tokens","children":[]},{"title":"APIs","path":"","children":[{"title":"Token Lifecycle","path":"payments/payment-methods/cards/token-hq/merchant-requestor-with-network-tokens/token-lifecycle","children":[]},{"title":"Tokenisation APIs","path":"payments/payment-methods/cards/token-hq/merchant-requestor-with-network-tokens/apis","children":[],"layout":"api"},{"title":"Token IIN API","path":"payments/payment-methods/cards/token-hq/merchant-requestor-with-network-tokens/iin-validation","children":[],"layout":"api"}],"layout":""},{"title":"CVV-less Flow","path":"payments/payment-methods/cards/token-hq/merchant-requestor-with-network-tokens/cvv-less-flow","children":[]},{"title":"Webhooks","path":"payments/payment-methods/cards/token-hq/merchant-requestor-with-network-tokens/webhooks","children":[],"layout":"api"},{"title":"Additional Information","path":"payments/payment-methods/cards/token-hq/merchant-requestor-with-network-tokens/additional-information","children":[]}]},{"title":"Tokenise Cards when Razorpay is Token Requestor","hidden":true,"children":[{"title":"Tokenise Cards when Razorpay is Token Requestor","path":"payments/payment-methods/cards/token-hq/razorpay-requestor-with-network-tokens","children":[]},{"title":"APIs","path":"","children":[{"title":"Token Lifecycle","path":"payments/payment-methods/cards/token-hq/razorpay-requestor-with-network-tokens/token-lifecycle","children":[]},{"title":"Tokenisation APIs","path":"payments/payment-methods/cards/token-hq/razorpay-requestor-with-network-tokens/apis","children":[],"layout":"api"},{"title":"IIN/BIN Validations on Tokens","path":"payments/payment-methods/cards/token-hq/razorpay-requestor-with-network-tokens/iin-validation","children":[],"layout":"api"}],"layout":""},{"title":"Tokenisation Webhooks","path":"payments/payment-methods/cards/token-hq/razorpay-requestor-with-network-tokens/webhooks","children":[]},{"title":"Additional Information","path":"payments/payment-methods/cards/token-hq/razorpay-requestor-with-network-tokens/additional-information","children":[]}]},{"title":"Pay Later - Custom Checkout","hidden":true,"children":[]},{"title":"Corporate Netbanking","hidden":true,"children":[{"title":"Corporate Netbanking","path":"payments/payment-methods/netbanking/corporate","children":[]}]},{"title":"Send GST information in UPI transaction flows","hidden":true,"children":[{"title":"Send GST information in UPI transaction flows","path":"payments/payment-methods/upi/gst-on-upi","children":[]},{"title":"FAQs","path":"payments/payment-methods/upi/gst-on-upi/faqs","children":[]}]},{"title":"Google Pay Integration - Custom Checkout","hidden":true,"children":[{"title":"Google Pay Integration - Custom Checkout","path":"payments/payment-methods/upi/google-pay/custom-integration","children":[]}]},{"title":"Google Spot Platform Integration","hidden":true,"children":[{"title":"Google Spot Platform Integration","path":"payments/payment-methods/upi/google-pay/spot-platform-integration","children":[]},{"title":"Custom Checkout Parameters","path":"payments/payment-methods/upi/google-pay/spot-platform-integration/checkout-parameters","children":[]}]},{"title":"Google Pay Omnichannel for Server-to-Server Integration","hidden":true,"children":[{"title":"Server-to-Server Integration","path":"payments/payment-methods/upi/google-pay/omnichannel/s2s-integration","children":[]}]},{"title":"Google Omnichannel Integration - Custom Checkout","hidden":true,"children":[{"title":"Google Omnichannel Integration - Custom Checkout","path":"payments/payment-methods/upi/google-pay/omnichannel/custom-integration","children":[]}]},{"title":"UPI Intent on iOS - S2S","hidden":true,"children":[{"title":"Server-to-Server Integration","path":"payments/payment-methods/upi/upi-intent/s2s-integration","children":[]}]},{"title":"List of External Wallets","hidden":true,"children":[]},{"title":"Paytm","hidden":true,"children":[{"title":"Paytm","path":"payments/payment-methods/wallets/paytm","children":[]}]},{"title":"Amazon Pay - Custom Checkout","hidden":true,"children":[]},{"title":"Cardless EMI - Custom Checkout","hidden":true,"children":[{"title":"Cardless EMI - Custom Checkout","path":"payments/payment-methods/emi/cardless-emi/custom-integration","children":[]}]},{"title":"Cardless EMI - S2S","hidden":true,"children":[]},{"title":"Highlight axio on Checkout","hidden":true,"children":[]},{"title":"axio Cardless EMI - Custom Checkout","hidden":true,"children":[]},{"title":"FAQs - axio","hidden":true,"children":[]},{"title":"S2S Integration","hidden":true,"children":[]},{"title":"No Cost EMIs from Bajaj Finserv - Custom Checkout","hidden":true,"children":[{"title":"No Cost EMIs from Bajaj Finserv - Custom Checkout","path":"payments/payment-methods/emi/no-cost-emi/bajaj-finserv/custom-integration","children":[]}]},{"title":"No Cost EMIs from Bajaj Finserv - S2S","hidden":true,"children":[]},{"title":"Account Code","hidden":true,"children":[{"title":"Account Code","path":"payments/route/account-code","children":[]},{"title":"Transfers API and Webhooks","path":"payments/route/account-code/api","children":[],"layout":"api"},{"title":"Dashboard","path":"payments/route/account-code/dashboard","children":[]}]},{"title":"Linked Accounts Creation Via Batch","hidden":true,"children":[]},{"title":"Other Features","hidden":true,"children":[]},{"title":"Pricing Model","hidden":true,"children":[]},{"title":"Direct Settlements","hidden":true,"children":[{"title":"Direct Settlements","path":"payments/settlements/direct","children":[]}]},{"title":"Third-Party Validation (TPV) - Custom Integration","hidden":true,"children":[{"title":"Third-Party Validation (TPV) - Custom Integration","path":"payments/third-party-validation/custom-integration","children":[]},{"title":"Best Practices","path":"payments/third-party-validation/custom-integration/best-practices","children":[]},{"title":"Supported Banks","path":"payments/third-party-validation/custom-integration/bank-list","children":[]}]},{"title":"Third-Party Validation (TPV) - S2S Integration","hidden":true,"children":[{"title":"Third-Party Validation (TPV) - S2S Integration","path":"payments/third-party-validation/s2s-integration","children":[]},{"title":"Payment Methods","path":"","children":[{"title":"Netbanking Integration","path":"payments/third-party-validation/s2s-integration/netbanking","children":[]},{"title":"UPI Collect Flow","path":"payments/third-party-validation/s2s-integration/upi/collect","children":[]},{"title":"UPI Intent Flow","path":"payments/third-party-validation/s2s-integration/upi/intent","children":[]},{"title":"Methods API","path":"payments/third-party-validation/s2s-integration/methods-api","children":[]}],"layout":""},{"title":"Supported Banks","path":"payments/third-party-validation/s2s-integration/bank-list","children":[]},{"title":"Best Practices","path":"payments/third-party-validation/s2s-integration/best-practices","children":[]}]},{"title":"Batch Creation","hidden":true,"children":[]},{"title":"API Endpoints","hidden":true,"children":[]},{"title":"Customer Identifier Status","hidden":true,"children":[]},{"title":"Test Payments in Smart Collect","hidden":true,"children":[]},{"title":"Update Expiry Date for an Individual Customer Identifier","hidden":true,"children":[{"title":"Update Customer Identifier Expiry Date in Bulk","path":"payments/smart-collect/update-expiry/bulk","children":[]},{"title":"Update Expiry Date for an Individual Customer Identifier","path":"payments/smart-collect/update-expiry","children":[]}]},{"title":"Update Expiry Date for an Individual Customer Identifier","hidden":true,"children":[{"title":"Update Expiry Date for an Individual Customer Identifier","path":"payments/smart-collect/update-individual-expiry","children":[]}]},{"title":"Razorpay Smart Collect","hidden":true,"children":[{"title":"Razorpay Smart Collect","path":"payments/smart-collect/va-vpa-qr","children":[]},{"title":"Notifications","path":"payments/smart-collect/va-vpa-qr/notification","children":[]},{"title":"Refunds","path":"payments/smart-collect/va-vpa-qr/refunds","children":[]},{"title":"Dashboard","path":"","children":[{"title":"About Smart Collect Dashboard","path":"payments/smart-collect/va-vpa-qr/dashboard","children":[]},{"title":"Create Customer Identifiers","path":"payments/smart-collect/va-vpa-qr/dashboard/create","children":[]},{"title":"Close Customer Identifier","path":"payments/smart-collect/va-vpa-qr/dashboard/close","children":[]},{"title":"Search Customer Identifier and Payments","path":"payments/smart-collect/va-vpa-qr/dashboard/search","children":[]},{"title":"Refund Payments","path":"payments/smart-collect/va-vpa-qr/dashboard/refund","children":[]},{"title":"Make Test Payments","path":"payments/smart-collect/va-vpa-qr/dashboard/test-payments","children":[]}],"layout":""},{"title":"FAQs","path":"payments/smart-collect/va-vpa-qr/faqs","children":[]},{"title":"Account Migration due to Yes Bank Moratorium","path":"payments/smart-collect/va-vpa-qr/yesbank-moratorium-migration","children":[]}]},{"title":"Customer Address API","hidden":true,"children":[]},{"title":"Coupon Codes APIs","hidden":true,"children":[]},{"title":"Shipping Info API","hidden":true,"children":[]},{"title":"80 G-enabled Payment Receipt","hidden":true,"children":[]},{"title":"Generic Payment Receipt","hidden":true,"children":[]},{"title":"Supported Platforms","hidden":true,"children":[]},{"title":"Add Facebook Pixel in Payment Success Page","hidden":true,"children":[]},{"title":"Integrate Payment Pages with Magic Checkout","hidden":true,"children":[]},{"title":"Cash Advance","hidden":true,"children":[]},{"title":"KYC Documents for Add-on Cards","hidden":true,"children":[]},{"title":"Working Capital Loans","hidden":true,"children":[]},{"title":"Approval Workflow","hidden":true,"children":[]},{"title":"RazorpayX - Delete QuickBooks Integration","hidden":true,"children":[{"title":"RazorpayX - Delete QuickBooks Integration","path":"x/quickbooks/delete","children":[]}]},{"title":"Manual TDS","hidden":true,"children":[]},{"title":"Approve Invoices","hidden":true,"children":[]},{"title":"Approvals On Invoices","hidden":true,"children":[]},{"title":"RazorpayX Vendor Portal","hidden":true,"children":[{"title":"RazorpayX Vendor Portal","path":"x/vendor-payments/portal","children":[]}]},{"title":"RazorpayX Payroll Integration with QuickBooks","hidden":true,"children":[]},{"title":"Time Management","hidden":true,"children":[]},{"title":"Cards Go Live on Recurring Payments","hidden":true,"children":[]},{"title":"Cards Tokenisation","hidden":true,"children":[{"title":"Cards Tokenisation","path":"announcements/rbi-card-mandate-guidelines/subscriptions/cards/tokenisation","children":[]}]}]
</script>
<script>
	window.__IS_HYDRATED__ = true;
    window.__TIMEOUT_NEEDED_FOR_SCROLL_TO_SECTION__ = true;
</script>
<script>
	window.__INITIAL_APP_STATE__ = {"org":"razorpay","country":"IN","initialColorScheme":"light"}
</script>

<script async src="https://www.googletagmanager.com/gtag/js?id=G-8HTFJ5WZ20"></script>
<script>
	window.dataLayer = window.dataLayer || [];
    function gtag(){dataLayer.push(arguments);}
    gtag('js', new Date());
    gtag('config', 'G-8HTFJ5WZ20');
    gtag('set', { 'countryCode' : 'IN', 'org' : 'razorpay' });
</script>

<style></style>
<style>
	@font-face {
		font-family: 'Lato';
		font-style: normal;
		font-weight: 400;
		// Keeping this option to avoid flicker due to font change, especially on slow network
		// Optional will wait 100ms for the font to load else will show fallback
		font-display: optional;
		src: url('/docs/build/browser/assets/fonts/lato-v22-latin-regular.woff2') format('woff2');
	}
</style>
<html lang="en">

<head>
	<meta charSet="utf-8" />
	<meta name="viewport" content="width=device-width, initial-scale=1" />
	<title data-rh="true">About Ecommerce Plugins | Razorpay Docs</title>
	<meta data-rh="true" property="og:title" content="About Ecommerce Plugins" />
	<meta data-rh="true" name="twitter:title" content="About Ecommerce Plugins" />
	<meta data-rh="true" name="description"
		content="Check the list of Razorpay Ecommerce Plugins to integrate with the plugin of your choice and accept payments from your customers." />
	<meta data-rh="true" property="og:description"
		content="Check the list of Razorpay Ecommerce Plugins to integrate with the plugin of your choice and accept payments from your customers." />
	<meta data-rh="true" name="twitter:description"
		content="Check the list of Razorpay Ecommerce Plugins to integrate with the plugin of your choice and accept payments from your customers." />
	<meta data-rh="true" property="og:type" content="website" />
	<meta data-rh="true" property="og:image" content="/docs/build/browser/static/og.18624133.png" />
	<meta data-rh="true" property="twitter:image" content="/docs/build/browser/static/og.18624133.png" />
	<meta data-rh="true" name="twitter:card" content="summary_large_image" />
	<meta data-rh="true" name="twitter:creator" content="Razorpay" />
	<meta data-rh="true" name="robots" content="index" />
	<meta data-rh="true" name="color-scheme" content="light" />
	<link data-rh="true" rel="shortcut icon" href="/favicon.png" type="image/png" />
	<link data-rh="true" rel="canonical" href="https://razorpay.com/payments/payment-gateway/ecommerce-plugins/" />
	<link rel="preload" href="/docs/build/browser/assets/fonts/lato-v22-latin-regular.woff2" as="font" type="font/woff2"
		crossorigin="anonymous" />
	<link data-chunk="main" rel="preload" as="script" href="/docs/build/browser/js/runtime.a17d3a71.js" />
	<link data-chunk="main" rel="preload" as="script" href="/docs/build/browser/js/51513.dedbf6a9.js" />
	<link data-chunk="main" rel="preload" as="script" href="/docs/build/browser/js/23825.0c60d07a.js" />
	<link data-chunk="main" rel="preload" as="script" href="/docs/build/browser/js/main.d0c7b243.js" />
	<style data-styled="" data-styled-version="5.3.1">
		.hHKSeB {
			box-sizing: border-box;
			display: block;
			background-color: hsla(0, 0%, 100%, 1);
			box-shadow: none;
			static;
			margin: 0;
			padding: 0;
			-webkit-flex: 0 1 auto;
			-ms-flex: 0 1 auto;
			flex: 0 1 auto;
		}

		/*!sc*/
		.cGOgLs {
			box-sizing: border-box;
			display: block;
			background-color: transparent;
			box-shadow: none;
			static;
			margin: 0;
			padding: 0;
			-webkit-flex: 0 1 auto;
			-ms-flex: 0 1 auto;
			flex: 0 1 auto;
		}

		/*!sc*/
		.lisYMx {
			box-sizing: border-box;
			display: none;
			background-color: hsla(0, 0%, 100%, 1);
			box-shadow: none;
			static;
			margin: 0;
			padding: 0;
			-webkit-flex: 0 1 auto;
			-ms-flex: 0 1 auto;
			flex: 0 1 auto;
			padding-left: 16px;
			padding-right: 16px;
			height: 56px;
			width: 100%;
		}

		/*!sc*/
		@media screen and (min-width:990px) {
			.lisYMx {
				display: -webkit-box;
				display: -webkit-flex;
				display: -ms-flexbox;
				display: flex;
			}
		}

		/*!sc*/
		@media screen and (min-width:1440px) {
			.lisYMx {
				padding-left: 40px;
			}
		}

		/*!sc*/
		@media screen and (min-width:1440px) {
			.lisYMx {
				padding-right: 40px;
			}
		}

		/*!sc*/
		.hFpJwV {
			box-sizing: border-box;
			display: -webkit-box;
			display: -webkit-flex;
			display: -ms-flexbox;
			display: flex;
			background-color: transparent;
			box-shadow: none;
			static;
			margin: 0;
			padding: 0;
			-webkit-flex: 1;
			-ms-flex: 1;
			flex: 1;
		}

		/*!sc*/
		.YlgZr {
			box-sizing: border-box;
			display: -webkit-box;
			display: -webkit-flex;
			display: -ms-flexbox;
			display: flex;
			background-color: transparent;
			box-shadow: none;
			static;
			margin: 0;
			padding: 0;
			-webkit-flex: 0 1 auto;
			-ms-flex: 0 1 auto;
			flex: 0 1 auto;
			width: 195px;
			height: 32px;
		}

		/*!sc*/
		.gHBrCZ {
			box-sizing: border-box;
			display: block;
			background-color: transparent;
			box-shadow: none;
			static;
			margin: 0;
			padding: 0;
			-webkit-flex: 0 1 auto;
			-ms-flex: 0 1 auto;
			flex: 0 1 auto;
			max-width: 195px;
			max-height: 32px;
		}

		/*!sc*/
		.bHbUpq {
			box-sizing: border-box;
			display: -webkit-box;
			display: -webkit-flex;
			display: -ms-flexbox;
			display: flex;
			background-color: transparent;
			box-shadow: none;
			position: relative;
			margin: 0;
			padding: 0;
			-webkit-flex: 1;
			-ms-flex: 1;
			flex: 1;
			width: -webkit-fit-content;
			width: -moz-fit-content;
			width: fit-content;
			max-width: 450px;
			border-width: 1px;
			border-radius: 4px;
			border-style: solid;
		}

		/*!sc*/
		.fiVOLr {
			box-sizing: border-box;
			display: -webkit-box;
			display: -webkit-flex;
			display: -ms-flexbox;
			display: flex;
			background-color: transparent;
			box-shadow: none;
			static;
			margin: 0;
			padding: 0;
			-webkit-flex: 0 1 auto;
			-ms-flex: 0 1 auto;
			flex: 0 1 auto;
			height: 32px;
		}

		/*!sc*/
		.ddVbIH {
			box-sizing: border-box;
			display: block;
			background-color: transparent;
			box-shadow: none;
			position: relative;
			margin: 0;
			padding: 0;
			-webkit-flex: 0 1 auto;
			-ms-flex: 0 1 auto;
			flex: 0 1 auto;
		}

		/*!sc*/
		.dPVYbu {
			box-sizing: border-box;
			display: -webkit-box;
			display: -webkit-flex;
			display: -ms-flexbox;
			display: flex;
			background-color: transparent;
			box-shadow: none;
			static;
			margin: 0;
			padding: 0;
			-webkit-flex: 0 1 auto;
			-ms-flex: 0 1 auto;
			flex: 0 1 auto;
		}

		/*!sc*/
		.gIjuDY {
			box-sizing: border-box;
			display: -webkit-box;
			display: -webkit-flex;
			display: -ms-flexbox;
			display: flex;
			background-color: transparent;
			box-shadow: none;
			static;
			margin: 0;
			padding: 0;
			-webkit-flex: 0 1 auto;
			-ms-flex: 0 1 auto;
			flex: 0 1 auto;
			padding-top: 4px;
			padding-bottom: 4px;
			height: 24px;
		}

		/*!sc*/
		.jObrhw {
			box-sizing: border-box;
			display: -webkit-box;
			display: -webkit-flex;
			display: -ms-flexbox;
			display: flex;
			background-color: transparent;
			box-shadow: none;
			static;
			margin: 0;
			padding: 0;
			-webkit-flex: 0 1 auto;
			-ms-flex: 0 1 auto;
			flex: 0 1 auto;
			height: 24px;
		}

		/*!sc*/
		.dWwBrM {
			box-sizing: border-box;
			display: block;
			background-color: transparent;
			box-shadow: none;
			static;
			margin: 0;
			padding: 0;
			-webkit-flex: 0 1 auto;
			-ms-flex: 0 1 auto;
			flex: 0 1 auto;
		}

		/*!sc*/
		@media screen and (min-width:990px) {
			.dWwBrM {
				display: none;
			}
		}

		/*!sc*/
		.fMFaKg {
			box-sizing: border-box;
			display: -webkit-box;
			display: -webkit-flex;
			display: -ms-flexbox;
			display: flex;
			background-color: transparent;
			box-shadow: none;
			static;
			margin: 0;
			padding: 0;
			-webkit-flex: 0 1 auto;
			-ms-flex: 0 1 auto;
			flex: 0 1 auto;
			padding: 0px;
			padding-left: 24px;
			padding-right: 16px;
			height: 56px;
			width: 100%;
		}

		/*!sc*/
		.btLJLX {
			box-sizing: border-box;
			display: -webkit-box;
			display: -webkit-flex;
			display: -ms-flexbox;
			display: flex;
			background-color: transparent;
			box-shadow: none;
			static;
			margin: 0;
			padding: 0;
			-webkit-flex: 0 1 auto;
			-ms-flex: 0 1 auto;
			flex: 0 1 auto;
			width: 140px;
			height: 32px;
		}

		/*!sc*/
		.veVFF {
			box-sizing: border-box;
			display: block;
			background-color: transparent;
			box-shadow: none;
			static;
			margin: 0;
			padding: 0;
			-webkit-flex: 0 1 auto;
			-ms-flex: 0 1 auto;
			flex: 0 1 auto;
			max-width: 140px;
			max-height: 32px;
		}

		/*!sc*/
		.jAGyDA {
			box-sizing: border-box;
			display: -webkit-box;
			display: -webkit-flex;
			display: -ms-flexbox;
			display: flex;
			background-color: transparent;
			box-shadow: none;
			static;
			margin: 0;
			padding: 0;
			-webkit-flex: 0 1 auto;
			-ms-flex: 0 1 auto;
			flex: 0 1 auto;
			padding-right: 4px;
			height: 32px;
		}

		/*!sc*/
		.bgUKhf {
			box-sizing: border-box;
			display: -webkit-box;
			display: -webkit-flex;
			display: -ms-flexbox;
			display: flex;
			background-color: transparent;
			box-shadow: none;
			static;
			margin: 0;
			padding: 0;
			-webkit-flex: 0 1 auto;
			-ms-flex: 0 1 auto;
			flex: 0 1 auto;
			width: 100%;
		}

		/*!sc*/
		.ixGcEy {
			box-sizing: border-box;
			display: none;
			background-color: transparent;
			box-shadow: none;
			position: -webkit-sticky;
			position: sticky;
			margin: 0;
			padding: 0;
			-webkit-flex: 0 1 auto;
			-ms-flex: 0 1 auto;
			flex: 0 1 auto;
			z-index: 1;
			top: 56px;
			width: -webkit-fit-content;
			width: -moz-fit-content;
			width: fit-content;
			height: calc(100vh - 56px);
		}

		/*!sc*/
		@media screen and (min-width:990px) {
			.ixGcEy {
				display: -webkit-box;
				display: -webkit-flex;
				display: -ms-flexbox;
				display: flex;
			}
		}

		/*!sc*/
		.ctYFNB {
			box-sizing: border-box;
			display: none;
			background-color: hsla(217, 56%, 17%, 1);
			box-shadow: none;
			static;
			margin: 0;
			padding: 0;
			-webkit-flex: 0 1 auto;
			-ms-flex: 0 1 auto;
			flex: 0 1 auto;
			width: 72px;
		}

		/*!sc*/
		@media screen and (min-width:990px) {
			.ctYFNB {
				display: block;
			}
		}

		/*!sc*/
		.dLhSPJ {
			box-sizing: border-box;
			display: -webkit-box;
			display: -webkit-flex;
			display: -ms-flexbox;
			display: flex;
			background-color: transparent;
			box-shadow: none;
			static;
			margin: 0;
			padding: 0;
			-webkit-flex: 0 1 auto;
			-ms-flex: 0 1 auto;
			flex: 0 1 auto;
			padding: 4px;
			width: 72px;
			height: 72px;
		}

		/*!sc*/
		.vOvvs {
			box-sizing: border-box;
			display: block;
			background-color: hsla(220, 27%, 98%, 1);
			box-shadow: none;
			position: relative;
			margin: 0;
			padding: 0;
			-webkit-flex: 0 1 auto;
			-ms-flex: 0 1 auto;
			flex: 0 1 auto;
			padding-left: 4px;
			padding-right: 16px;
			padding-top: 12px;
			padding-bottom: 20px;
			width: 256px;
			height: calc(100%);
			overflow: auto;
		}

		/*!sc*/
		.bQnGvS {
			box-sizing: border-box;
			display: block;
			background-color: transparent;
			box-shadow: none;
			static;
			margin: 0;
			padding: 0;
			-webkit-flex: 0 1 auto;
			-ms-flex: 0 1 auto;
			flex: 0 1 auto;
			padding-left: 24px;
			padding-top: 8px;
			padding-bottom: 8px;
		}

		/*!sc*/
		.jiMkSI {
			box-sizing: border-box;
			display: block;
			background-color: transparent;
			box-shadow: none;
			static;
			margin: 0;
			padding: 0;
			-webkit-flex: 0 1 auto;
			-ms-flex: 0 1 auto;
			flex: 0 1 auto;
			padding-top: 4px;
			padding-bottom: 4px;
		}

		/*!sc*/
		.jnDyMP {
			box-sizing: border-box;
			display: -webkit-box;
			display: -webkit-flex;
			display: -ms-flexbox;
			display: flex;
			background-color: transparent;
			box-shadow: none;
			position: relative;
			margin: 0;
			padding: 0;
			-webkit-flex: 0 1 auto;
			-ms-flex: 0 1 auto;
			flex: 0 1 auto;
			padding-top: 8px;
			padding-bottom: 8px;
			padding-left: 24px;
		}

		/*!sc*/
		.hZRMgn {
			box-sizing: border-box;
			display: block;
			background-color: transparent;
			box-shadow: none;
			position: absolute;
			margin: 0;
			padding: 0;
			-webkit-flex: 0 1 auto;
			-ms-flex: 0 1 auto;
			flex: 0 1 auto;
			top: 7px;
			left: 8px;
		}

		/*!sc*/
		.iFgnvD {
			box-sizing: border-box;
			display: block;
			background-color: transparent;
			box-shadow: none;
			static;
			margin: 0;
			padding: 0;
			-webkit-flex: 0 1 auto;
			-ms-flex: 0 1 auto;
			flex: 0 1 auto;
			padding-left: 12px;
		}

		/*!sc*/
		.iANuVs {
			box-sizing: border-box;
			display: -webkit-box;
			display: -webkit-flex;
			display: -ms-flexbox;
			display: flex;
			background-color: transparent;
			box-shadow: none;
			static;
			margin: 0;
			padding: 0;
			-webkit-flex: 1;
			-ms-flex: 1;
			flex: 1;
			width: calc(100% - 328px);
		}

		/*!sc*/
		.dGChSs {
			box-sizing: border-box;
			display: -webkit-box;
			display: -webkit-flex;
			display: -ms-flexbox;
			display: flex;
			background-color: transparent;
			box-shadow: none;
			static;
			margin: 0;
			padding: 0;
			-webkit-flex: 1;
			-ms-flex: 1;
			flex: 1;
			width: 100%;
			min-height: calc(100% - 112px);
		}

		/*!sc*/
		.NWmfY {
			box-sizing: border-box;
			display: -webkit-box;
			display: -webkit-flex;
			display: -ms-flexbox;
			display: flex;
			background-color: transparent;
			box-shadow: none;
			static;
			margin: 0;
			padding: 0;
			-webkit-flex: 0 1 auto;
			-ms-flex: 0 1 auto;
			flex: 0 1 auto;
			padding-top: 56px;
			padding-bottom: 56px;
			padding-left: 16px;
			padding-right: 16px;
			width: min(100%, 768px);
		}

		/*!sc*/
		@media screen and (min-width:990px) {
			.NWmfY {
				padding-left: 24px;
			}
		}

		/*!sc*/
		@media screen and (min-width:1200px) {
			.NWmfY {
				padding-left: 40px;
			}
		}

		/*!sc*/
		@media screen and (min-width:990px) {
			.NWmfY {
				padding-right: 24px;
			}
		}

		/*!sc*/
		@media screen and (min-width:1200px) {
			.NWmfY {
				padding-right: 40px;
			}
		}

		/*!sc*/
		@media screen and (min-width:1200px) {
			.NWmfY {
				width: min(calc(100% - 240px), 768px);
			}
		}

		/*!sc*/
		.dWYgks {
			box-sizing: border-box;
			display: block;
			background-color: transparent;
			box-shadow: none;
			static;
			margin: 0;
			padding: 0;
			-webkit-flex: 1;
			-ms-flex: 1;
			flex: 1;
			padding-bottom: 56px;
		}

		/*!sc*/
		.ldkSSq {
			box-sizing: border-box;
			display: -webkit-box;
			display: -webkit-flex;
			display: -ms-flexbox;
			display: flex;
			background-color: transparent;
			box-shadow: none;
			position: relative;
			margin: 0;
			padding: 0;
			-webkit-flex: 0 1 auto;
			-ms-flex: 0 1 auto;
			flex: 0 1 auto;
			overflow-x: auto;
		}

		/*!sc*/
		.gbWiaG {
			box-sizing: border-box;
			display: -webkit-box;
			display: -webkit-flex;
			display: -ms-flexbox;
			display: flex;
			background-color: transparent;
			box-shadow: none;
			static;
			margin: 0;
			padding: 0;
			-webkit-flex: 0 1 auto;
			-ms-flex: 0 1 auto;
			flex: 0 1 auto;
			padding-bottom: 8px;
		}

		/*!sc*/
		.hAURWq {
			box-sizing: border-box;
			display: block;
			background-color: transparent;
			box-shadow: none;
			static;
			margin: 0;
			padding: 0;
			-webkit-flex: 0 1 auto;
			-ms-flex: 0 1 auto;
			flex: 0 1 auto;
			padding-bottom: 24px;
		}

		/*!sc*/
		.lpjypG {
			box-sizing: border-box;
			display: -webkit-inline-box;
			display: -webkit-inline-flex;
			display: -ms-inline-flexbox;
			display: inline-flex;
			background-color: transparent;
			box-shadow: none;
			static;
			margin: 0;
			padding: 0;
			-webkit-flex: 0 1 auto;
			-ms-flex: 0 1 auto;
			flex: 0 1 auto;
		}

		/*!sc*/
		.kHUkaB {
			box-sizing: border-box;
			display: -webkit-box;
			display: -webkit-flex;
			display: -ms-flexbox;
			display: flex;
			background-color: transparent;
			box-shadow: none;
			static;
			margin: 0;
			padding: 0;
			-webkit-flex: 0 1 auto;
			-ms-flex: 0 1 auto;
			flex: 0 1 auto;
			min-width: 256px;
		}

		/*!sc*/
		.dcjpbN {
			box-sizing: border-box;
			display: -webkit-box;
			display: -webkit-flex;
			display: -ms-flexbox;
			display: flex;
			background-color: transparent;
			box-shadow: none;
			position: relative;
			margin: 0;
			padding: 0;
			-webkit-flex: 0 1 auto;
			-ms-flex: 0 1 auto;
			flex: 0 1 auto;
			width: 100%;
			border: 1px solid hsla(216, 15%, 54%, 0.09);
		}

		/*!sc*/
		.igNNgb {
			box-sizing: border-box;
			display: none;
			background-color: transparent;
			box-shadow: none;
			position: -webkit-sticky;
			position: sticky;
			margin: 0;
			padding: 0;
			-webkit-flex: 0 1 auto;
			-ms-flex: 0 1 auto;
			flex: 0 1 auto;
			top: 56px;
			padding-top: 56px;
			padding-bottom: 56px;
			width: 240px;
			height: calc(100vh - 68px);
		}

		/*!sc*/
		@media screen and (min-width:1200px) {
			.igNNgb {
				display: -webkit-box;
				display: -webkit-flex;
				display: -ms-flexbox;
				display: flex;
			}
		}

		/*!sc*/
		.foKBkC {
			box-sizing: border-box;
			display: block;
			background-color: transparent;
			box-shadow: none;
			static;
			margin: 0;
			padding: 0;
			-webkit-flex: 100 1 0;
			-ms-flex: 100 1 0;
			flex: 100 1 0;
			padding-left: 16px;
			padding-right: 16px;
			padding-top: 40px;
			overflow: hidden;
		}

		/*!sc*/
		.llIhct {
			box-sizing: border-box;
			display: -webkit-box;
			display: -webkit-flex;
			display: -ms-flexbox;
			display: flex;
			background-color: transparent;
			box-shadow: none;
			static;
			margin: 0;
			padding: 0;
			-webkit-flex: 0 1 auto;
			-ms-flex: 0 1 auto;
			flex: 0 1 auto;
			height: 100%;
			overflow-y: hidden;
		}

		/*!sc*/
		.eaPebU {
			box-sizing: border-box;
			display: block;
			background-color: transparent;
			box-shadow: none;
			static;
			margin: 0;
			padding: 0;
			-webkit-flex: 0 1 auto;
			-ms-flex: 0 1 auto;
			flex: 0 1 auto;
			padding-top: 4px;
			padding-bottom: 8px;
			border-width: 0px;
			border-left-width: 1px;
			border-style: solid;
			border-color: hsla(216, 15%, 54%, 0.18);
		}

		/*!sc*/
		.hUQOpC {
			box-sizing: border-box;
			display: -webkit-box;
			display: -webkit-flex;
			display: -ms-flexbox;
			display: flex;
			background-color: transparent;
			box-shadow: none;
			static;
			margin: 0;
			padding: 0;
			-webkit-flex: 1 0 auto;
			-ms-flex: 1 0 auto;
			flex: 1 0 auto;
		}

		/*!sc*/
		.iKxIPs {
			box-sizing: border-box;
			display: block;
			background-color: transparent;
			box-shadow: none;
			position: fixed;
			margin: 0;
			padding: 0;
			-webkit-flex: 0 1 auto;
			-ms-flex: 0 1 auto;
			flex: 0 1 auto;
			right: 24px;
			bottom: 24px;
			width: -webkit-fit-content;
			width: -moz-fit-content;
			width: fit-content;
		}

		/*!sc*/
		.iXFBBH {
			box-sizing: border-box;
			display: -webkit-box;
			display: -webkit-flex;
			display: -ms-flexbox;
			display: flex;
			background-color: transparent;
			box-shadow: none;
			static;
			margin: 0;
			padding: 0;
			-webkit-flex: 0 1 auto;
			-ms-flex: 0 1 auto;
			flex: 0 1 auto;
			padding: 0px;
		}

		/*!sc*/
		@media screen and (min-width:990px) {
			.iXFBBH {
				padding: 8px;
			}
		}

		/*!sc*/
		.kkSa-dm {
			box-sizing: border-box;
			display: -webkit-box;
			display: -webkit-flex;
			display: -ms-flexbox;
			display: flex;
			background-color: transparent;
			box-shadow: none;
			static;
			margin: 0;
			padding: 0;
			-webkit-flex: 0 1 auto;
			-ms-flex: 0 1 auto;
			flex: 0 1 auto;
			width: 40px;
			height: 40px;
		}

		/*!sc*/
		@media screen and (min-width:990px) {
			.kkSa-dm {
				width: 32px;
			}
		}

		/*!sc*/
		@media screen and (min-width:990px) {
			.kkSa-dm {
				height: 32px;
			}
		}

		/*!sc*/
		data-styled.g1[id="Box-sc-5vx4ls-0"] {
			content: "hHKSeB,cGOgLs,lisYMx,hFpJwV,YlgZr,gHBrCZ,bHbUpq,fiVOLr,ddVbIH,dPVYbu,gIjuDY,jObrhw,dWwBrM,fMFaKg,btLJLX,veVFF,jAGyDA,bgUKhf,ixGcEy,ctYFNB,dLhSPJ,vOvvs,bQnGvS,jiMkSI,jnDyMP,hZRMgn,iFgnvD,iANuVs,dGChSs,NWmfY,dWYgks,ldkSSq,gbWiaG,hAURWq,lpjypG,kHUkaB,dcjpbN,igNNgb,foKBkC,llIhct,eaPebU,hUQOpC,iKxIPs,iXFBBH,kkSa-dm,"
		}

		/*!sc*/
		.dCZIGP {
			display: -webkit-box;
			display: -webkit-flex;
			display: -ms-flexbox;
			display: flex;
			-webkit-align-items: center;
			-webkit-box-align: center;
			-ms-flex-align: center;
			align-items: center;
			position: relative;
		}

		/*!sc*/
		.hNwRVL {
			padding-top: 40px;
			padding-bottom: 40px;
		}

		/*!sc*/
		data-styled.g2[id="BaseBoxweb__BaseBox-sc-1icfu8j-0"] {
			content: "dCZIGP,hNwRVL,"
		}

		/*!sc*/
		.bRSBxk {
			position: absolute;
			right: 16px;
			display: -webkit-box;
			display: -webkit-flex;
			display: -ms-flexbox;
			display: flex;
			width: 20px;
			height: 20px;
			-webkit-align-items: center;
			-webkit-box-align: center;
			-ms-flex-align: center;
			align-items: center;
			-webkit-box-pack: center;
			-webkit-justify-content: center;
			-ms-flex-pack: center;
			justify-content: center;
			border-radius: 2px;
			color: hsla(214, 18%, 69%, 1);
			border: 1px solid hsla(216, 15%, 54%, 0.18);
			background: hsla(220, 30%, 96%, 1);
		}

		/*!sc*/
		.bRSBxk span {
			height: 20px;
		}

		/*!sc*/
		data-styled.g22[id="SearchRight__SearchRightContainer-sc-9nccfz-0"] {
			content: "bRSBxk,"
		}

		/*!sc*/
		.jyrMiD {
			color: hsla(216, 27%, 36%, 1);
			margin: 0;
			padding: 0;
			font-size: 14px;
			font-weight: 400;
			font-family: Lato, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol";
			padding-left: 0px;
			padding-right: 0px;
		}

		/*!sc*/
		.kgsGEf {
			color: hsla(216, 27%, 36%, 1);
			margin: 0;
			padding: 0;
			font-size: 14px;
			font-weight: 400;
			font-family: Lato, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol";
			padding-left: 16px;
			padding-right: 16px;
		}

		/*!sc*/
		.HSevc {
			color: hsla(216, 27%, 36%, 1);
			margin: 0;
			padding: 0;
			font-size: 14px;
			font-weight: 400;
			font-family: Lato, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol";
		}

		/*!sc*/
		.cmLnxL {
			color: hsla(0, 0%, 100%, 1);
			margin: 0;
			padding: 0;
			font-size: 12px;
			font-weight: 400;
			font-family: Lato, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol";
			text-align: center;
			line-height: 16px;
			padding-top: 4px;
		}

		/*!sc*/
		.bsHdmV {
			color: hsla(216, 27%, 36%, 1);
			margin: 0;
			padding: 0;
			font-size: 14px;
			font-weight: 400;
			font-family: Lato, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol";
			line-height: 16px;
		}

		/*!sc*/
		.ieCmBj {
			color: hsla(216, 27%, 36%, 1);
			margin: 0;
			padding: 0;
			font-size: 14px;
			font-weight: 700;
			font-family: Lato, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol";
		}

		/*!sc*/
		.cnaGRq {
			color: hsla(216, 27%, 36%, 1);
			margin: 0;
			padding: 0;
			font-size: 14px;
			font-weight: 700;
			font-family: Lato, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol";
			line-height: 16px;
		}

		/*!sc*/
		.ifSOxV {
			color: hsla(216, 27%, 36%, 1);
			margin: 0;
			padding: 0;
			font-size: 12px;
			font-weight: 400;
			font-family: Lato, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol";
			padding-left: 0px;
			padding-right: 0px;
		}

		/*!sc*/
		.jzJcTI {
			color: hsla(217, 18%, 45%, 1);
			margin: 0;
			padding: 0;
			font-size: 12px;
			font-weight: 700;
			font-family: Lato, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol";
			text-align: center;
		}

		/*!sc*/
		.gqQyhM {
			color: hsla(217, 18%, 45%, 1);
			margin: 0;
			padding: 0;
			font-size: 20px;
			font-weight: 400;
			font-family: Lato, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol";
			line-height: 30px;
			padding-top: 4px;
			padding-bottom: 16px;
		}

		/*!sc*/
		.fhcimu {
			color: hsla(216, 27%, 36%, 1);
			margin: 0;
			padding: 0;
			font-size: 16px;
			font-weight: 400;
			font-family: Lato, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol";
		}

		/*!sc*/
		.bNBVOX {
			color: hsla(216, 27%, 36%, 1);
			margin: 0;
			padding: 0;
			font-size: 14px;
			font-weight: 400;
			font-family: Lato, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol";
			padding-right: 8px;
		}

		/*!sc*/
		.dePkrl {
			color: hsla(216, 27%, 36%, 1);
			margin: 0;
			padding: 0;
			font-size: 16px;
			font-weight: 400;
			font-family: Lato, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol";
			padding-left: 0;
			padding-right: 0;
		}

		/*!sc*/
		.ikQWpa {
			color: hsla(217, 56%, 17%, 1);
			margin: 0;
			padding: 0;
			font-size: 16px;
			font-weight: 700;
			font-family: Lato, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol";
			line-height: 32px;
		}

		/*!sc*/
		.ckbwmr {
			color: hsla(216, 27%, 36%, 1);
			margin: 0;
			padding: 0;
			font-size: 14px;
			font-weight: 400;
			font-family: Lato, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol";
			padding-top: 40px;
			padding-bottom: 16px;
		}

		/*!sc*/
		.IPzaW {
			color: hsla(216, 27%, 36%, 1);
			margin: 0;
			padding: 0;
			font-size: 12px;
			font-weight: 400;
			font-family: Lato, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol";
		}

		/*!sc*/
		.dWSCQs {
			color: hsla(8, 73%, 47%, 1);
			margin: 0;
			padding: 0;
			font-size: 12px;
			font-weight: 400;
			font-family: Lato, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol";
			padding-top: 8px;
			padding-left: 8px;
		}

		/*!sc*/
		.bjKbMn {
			color: hsla(216, 27%, 36%, 1);
			margin: 0;
			padding: 0;
			font-size: 14px;
			font-weight: 400;
			font-family: Lato, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol";
			padding-left: 0px;
			padding-right: 8px;
		}

		/*!sc*/
		.erLHrN {
			color: hsla(216, 16%, 60%, 1);
			margin: 0;
			padding: 0;
			font-size: 14px;
			font-weight: 400;
			font-family: Lato, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol";
			text-transform: uppercase;
			padding-left: 8px;
		}

		/*!sc*/
		.iKTxur {
			color: hsla(216, 27%, 36%, 1);
			margin: 0;
			padding: 0;
			font-size: 14px;
			font-weight: 400;
			font-family: Lato, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol";
			padding-left: 8px;
			padding-right: 4px;
		}

		/*!sc*/
		data-styled.g23[id="Text-sc-1g8cvhx-0"] {
			content: "jyrMiD,kgsGEf,HSevc,cmLnxL,bsHdmV,ieCmBj,cnaGRq,ifSOxV,jzJcTI,gqQyhM,fhcimu,bNBVOX,dePkrl,ikQWpa,ckbwmr,IPzaW,dWSCQs,bjKbMn,erLHrN,iKTxur,"
		}

		/*!sc*/
		.bNqftg {
			-webkit-box-pack: justify;
			-webkit-justify-content: space-between;
			-ms-flex-pack: justify;
			justify-content: space-between;
			-webkit-align-items: center;
			-webkit-box-align: center;
			-ms-flex-align: center;
			align-items: center;
			gap: 0px 0px;
			-webkit-column-gap: 16px;
			column-gap: 16px;
			-webkit-flex-wrap: nowrap;
			-ms-flex-wrap: nowrap;
			flex-wrap: nowrap;
		}

		/*!sc*/
		.fCPAWO {
			-webkit-box-pack: start;
			-webkit-justify-content: flex-start;
			-ms-flex-pack: start;
			justify-content: flex-start;
			-webkit-align-items: center;
			-webkit-box-align: center;
			-ms-flex-align: center;
			align-items: center;
			gap: 0px 0px;
			-webkit-flex-wrap: nowrap;
			-ms-flex-wrap: nowrap;
			flex-wrap: nowrap;
		}

		/*!sc*/
		.jcarLi {
			-webkit-box-pack: start;
			-webkit-justify-content: flex-start;
			-ms-flex-pack: start;
			justify-content: flex-start;
			-webkit-flex-direction: row;
			-ms-flex-direction: row;
			flex-direction: row;
			-webkit-align-items: center;
			-webkit-box-align: center;
			-ms-flex-align: center;
			align-items: center;
			gap: 0px 0px;
			-webkit-flex-wrap: nowrap;
			-ms-flex-wrap: nowrap;
			flex-wrap: nowrap;
		}

		/*!sc*/
		.kNUFIs {
			-webkit-box-pack: start;
			-webkit-justify-content: flex-start;
			-ms-flex-pack: start;
			justify-content: flex-start;
			-webkit-align-items: center;
			-webkit-box-align: center;
			-ms-flex-align: center;
			align-items: center;
			gap: 0px 0px;
			-webkit-column-gap: 24px;
			column-gap: 24px;
			-webkit-flex-wrap: nowrap;
			-ms-flex-wrap: nowrap;
			flex-wrap: nowrap;
		}

		/*!sc*/
		.foqTwv {
			-webkit-box-pack: start;
			-webkit-justify-content: flex-start;
			-ms-flex-pack: start;
			justify-content: flex-start;
			gap: 0px 0px;
			-webkit-column-gap: 24px;
			column-gap: 24px;
			-webkit-flex-wrap: nowrap;
			-ms-flex-wrap: nowrap;
			flex-wrap: nowrap;
		}

		/*!sc*/
		.ldIsSH {
			-webkit-box-pack: justify;
			-webkit-justify-content: space-between;
			-ms-flex-pack: justify;
			justify-content: space-between;
			-webkit-align-items: center;
			-webkit-box-align: center;
			-ms-flex-align: center;
			align-items: center;
			gap: 0px 0px;
			-webkit-flex-wrap: nowrap;
			-ms-flex-wrap: nowrap;
			flex-wrap: nowrap;
		}

		/*!sc*/
		.ekisLk {
			-webkit-box-pack: center;
			-webkit-justify-content: center;
			-ms-flex-pack: center;
			justify-content: center;
			gap: 0px 0px;
			-webkit-flex-wrap: nowrap;
			-ms-flex-wrap: nowrap;
			flex-wrap: nowrap;
		}

		/*!sc*/
		.gbpuuV {
			-webkit-box-pack: start;
			-webkit-justify-content: flex-start;
			-ms-flex-pack: start;
			justify-content: flex-start;
			gap: 0px 0px;
			-webkit-flex-wrap: nowrap;
			-ms-flex-wrap: nowrap;
			flex-wrap: nowrap;
		}

		/*!sc*/
		.enkULn {
			-webkit-box-pack: center;
			-webkit-justify-content: center;
			-ms-flex-pack: center;
			justify-content: center;
			-webkit-flex-direction: column;
			-ms-flex-direction: column;
			flex-direction: column;
			-webkit-align-items: center;
			-webkit-box-align: center;
			-ms-flex-align: center;
			align-items: center;
			gap: 0px 0px;
			-webkit-flex-wrap: nowrap;
			-ms-flex-wrap: nowrap;
			flex-wrap: nowrap;
		}

		/*!sc*/
		.kqsqjK {
			-webkit-box-pack: start;
			-webkit-justify-content: flex-start;
			-ms-flex-pack: start;
			justify-content: flex-start;
			-webkit-align-items: baseline;
			-webkit-box-align: baseline;
			-ms-flex-align: baseline;
			align-items: baseline;
			gap: 0px 0px;
			-webkit-flex-wrap: nowrap;
			-ms-flex-wrap: nowrap;
			flex-wrap: nowrap;
		}

		/*!sc*/
		.gyXFoV {
			-webkit-box-pack: start;
			-webkit-justify-content: flex-start;
			-ms-flex-pack: start;
			justify-content: flex-start;
			-webkit-flex-direction: column;
			-ms-flex-direction: column;
			flex-direction: column;
			gap: 0px 0px;
			-webkit-flex-wrap: nowrap;
			-ms-flex-wrap: nowrap;
			flex-wrap: nowrap;
		}

		/*!sc*/
		.fwnSqg {
			-webkit-box-pack: center;
			-webkit-justify-content: center;
			-ms-flex-pack: center;
			justify-content: center;
			-webkit-flex-direction: column;
			-ms-flex-direction: column;
			flex-direction: column;
			gap: 0px 0px;
			-webkit-column-gap: 40px;
			column-gap: 40px;
			-webkit-flex-wrap: nowrap;
			-ms-flex-wrap: nowrap;
			flex-wrap: nowrap;
		}

		/*!sc*/
		.eFTsHp {
			-webkit-box-pack: start;
			-webkit-justify-content: flex-start;
			-ms-flex-pack: start;
			justify-content: flex-start;
			gap: 0px 0px;
			-webkit-column-gap: 8px;
			column-gap: 8px;
			-webkit-flex-wrap: nowrap;
			-ms-flex-wrap: nowrap;
			flex-wrap: nowrap;
		}

		/*!sc*/
		.knXDpV {
			-webkit-box-pack: justify;
			-webkit-justify-content: space-between;
			-ms-flex-pack: justify;
			justify-content: space-between;
			-webkit-flex-direction: column;
			-ms-flex-direction: column;
			flex-direction: column;
			gap: 0px 0px;
			row-gap: 16px;
			-webkit-column-gap: 16px;
			column-gap: 16px;
			-webkit-flex-wrap: nowrap;
			-ms-flex-wrap: nowrap;
			flex-wrap: nowrap;
		}

		/*!sc*/
		@media screen and (min-width:550px) {
			.knXDpV {
				-webkit-flex-direction: row;
				-ms-flex-direction: row;
				flex-direction: row;
			}
		}

		/*!sc*/
		.jKPpuE {
			-webkit-box-pack: start;
			-webkit-justify-content: flex-start;
			-ms-flex-pack: start;
			justify-content: flex-start;
			gap: 0px 0px;
			-webkit-flex-wrap: wrap;
			-ms-flex-wrap: wrap;
			flex-wrap: wrap;
		}

		/*!sc*/
		.tGMIa {
			-webkit-box-pack: start;
			-webkit-justify-content: flex-start;
			-ms-flex-pack: start;
			justify-content: flex-start;
			-webkit-flex-direction: column;
			-ms-flex-direction: column;
			flex-direction: column;
			gap: 0px 0px;
			row-gap: 16px;
			-webkit-flex-wrap: nowrap;
			-ms-flex-wrap: nowrap;
			flex-wrap: nowrap;
		}

		/*!sc*/
		.hDYGnW {
			-webkit-box-pack: start;
			-webkit-justify-content: flex-start;
			-ms-flex-pack: start;
			justify-content: flex-start;
			-webkit-align-items: center;
			-webkit-box-align: center;
			-ms-flex-align: center;
			align-items: center;
			gap: 0px 0px;
			-webkit-column-gap: 8px;
			column-gap: 8px;
			-webkit-flex-wrap: nowrap;
			-ms-flex-wrap: nowrap;
			flex-wrap: nowrap;
		}

		/*!sc*/
		.fxAeXL {
			-webkit-box-pack: center;
			-webkit-justify-content: center;
			-ms-flex-pack: center;
			justify-content: center;
			-webkit-align-items: center;
			-webkit-box-align: center;
			-ms-flex-align: center;
			align-items: center;
			gap: 0px 0px;
			-webkit-flex-wrap: nowrap;
			-ms-flex-wrap: nowrap;
			flex-wrap: nowrap;
		}

		/*!sc*/
		data-styled.g24[id="Flex__StyledFlex-sc-1n8gmmd-0"] {
			content: "bNqftg,fCPAWO,jcarLi,kNUFIs,foqTwv,ldIsSH,ekisLk,gbpuuV,enkULn,kqsqjK,gyXFoV,fwnSqg,eFTsHp,knXDpV,jKPpuE,tGMIa,hDYGnW,fxAeXL,"
		}

		/*!sc*/
		.kWnpZi {
			cursor: pointer;
		}

		/*!sc*/
		.kWnpZi a {
			-webkit-text-decoration: none;
			text-decoration: none;
			outline: none;
		}

		/*!sc*/
		data-styled.g25[id="Link__StyledLink-sc-38tiy-0"] {
			content: "kWnpZi,"
		}

		/*!sc*/
		.fLetpi {
			color: hsla(213, 89%, 56%, 1);
			-webkit-transition: color 100ms ease-in-out;
			transition: color 100ms ease-in-out;
		}

		/*!sc*/
		.Link__StyledLink-sc-38tiy-0:hover .Link__StyledText-sc-38tiy-2 {
			color: hsla(218, 89%, 51%, 1);
		}

		/*!sc*/
		.Link__StyledLink-sc-38tiy-0:focus .Link__StyledText-sc-38tiy-2 {
			color: hsla(223, 95%, 48%, 1);
		}

		/*!sc*/
		.Link__StyledLink-sc-38tiy-0:active .Link__StyledText-sc-38tiy-2 {
			color: hsla(223, 95%, 48%, 1);
		}

		/*!sc*/
		.SCkGc {
			color: hsla(216, 16%, 60%, 1);
			-webkit-transition: color 100ms ease-in-out;
			transition: color 100ms ease-in-out;
		}

		/*!sc*/
		.Link__StyledLink-sc-38tiy-0:hover .Link__StyledText-sc-38tiy-2 {
			color: hsla(218, 89%, 51%, 1);
		}

		/*!sc*/
		.Link__StyledLink-sc-38tiy-0:focus .Link__StyledText-sc-38tiy-2 {
			color: hsla(223, 95%, 48%, 1);
		}

		/*!sc*/
		.Link__StyledLink-sc-38tiy-0:active .Link__StyledText-sc-38tiy-2 {
			color: hsla(223, 95%, 48%, 1);
		}

		/*!sc*/
		.kkMCYI {
			color: hsla(217, 18%, 45%, 1);
			-webkit-transition: color 100ms ease-in-out;
			transition: color 100ms ease-in-out;
		}

		/*!sc*/
		.Link__StyledLink-sc-38tiy-0:hover .Link__StyledText-sc-38tiy-2 {
			color: hsla(218, 89%, 51%, 1);
		}

		/*!sc*/
		.Link__StyledLink-sc-38tiy-0:focus .Link__StyledText-sc-38tiy-2 {
			color: hsla(223, 95%, 48%, 1);
		}

		/*!sc*/
		.Link__StyledLink-sc-38tiy-0:active .Link__StyledText-sc-38tiy-2 {
			color: hsla(223, 95%, 48%, 1);
		}

		/*!sc*/
		data-styled.g27[id="Link__StyledText-sc-38tiy-2"] {
			content: "fLetpi,SCkGc,kkMCYI,"
		}

		/*!sc*/
		@media (max-width:550px) {
			.bjYPIl:before {
				visibility: hidden;
				opacity: 0;
				-webkit-transition: visibility 0.2s, opacity 0.2s linear;
				transition: visibility 0.2s, opacity 0.2s linear;
				content: '';
				position: fixed;
				width: 16px;
				height: 24px;
				left: 15px;
				background: linear-gradient(90deg, #FFFFFF 0%, rgba(255, 255, 255, 0.7) 50%);
			}

			.bjYPIl:after {
				visibility: hidden;
				opacity: 0;
				-webkit-transition: visibility 0.2s, opacity 0.2s linear;
				transition: visibility 0.2s, opacity 0.2s linear;
				content: '';
				position: fixed;
				width: 16px;
				height: 24px;
				right: 15px;
				background: linear-gradient(90deg, #FFFFFF 0%, rgba(255, 255, 255, 0.7) 50%);
			}
		}

		/*!sc*/
		.bjYPIl .Link__StyledLink-sc-38tiy-0 {
			-webkit-flex-shrink: 0;
			-ms-flex-negative: 0;
			flex-shrink: 0;
			text-align: center;
		}

		/*!sc*/
		.bjYPIl .Link__StyledLink-sc-38tiy-0:not(:last-child):after {
			content: '/';
			padding: 4px;
			color: hsla(216, 16%, 60%, 1);
		}

		/*!sc*/
		data-styled.g28[id="styled__StyledBreadcrumbsContainer-sc-mcrmsw-0"] {
			content: "bjYPIl,"
		}

		/*!sc*/
		.fsUibx {
			-webkit-flex-shrink: 0;
			-ms-flex-negative: 0;
			flex-shrink: 0;
		}

		/*!sc*/
		.fsUibx:not(:last-child):after {
			content: '/';
			padding: 4px;
			color: hsla(216, 16%, 60%, 1);
		}

		/*!sc*/
		data-styled.g29[id="styled__StyledTextContainer-sc-mcrmsw-1"] {
			content: "fsUibx,"
		}

		/*!sc*/
		.kZQjgd {
			-webkit-scroll-margin-top: 56px;
			-moz-scroll-margin-top: 56px;
			-ms-scroll-margin-top: 56px;
			scroll-margin-top: 56px;
			color: hsla(217, 56%, 17%, 1);
			margin: 0;
			padding: 0;
			line-height: 60px;
			text-align: initial;
			font-size: 40px;
			font-weight: 700;
			font-family: Lato, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol";
			padding-top: 12px;
			padding-bottom: 0px;
		}

		/*!sc*/
		.RtGqJ {
			-webkit-scroll-margin-top: 56px;
			-moz-scroll-margin-top: 56px;
			-ms-scroll-margin-top: 56px;
			scroll-margin-top: 56px;
			color: hsla(217, 56%, 17%, 1);
			margin: 0;
			padding: 0;
			line-height: 1;
			text-align: initial;
			font-size: 40px;
			font-weight: 700;
			font-family: Lato, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol";
		}

		/*!sc*/
		data-styled.g30[id="Heading__StyledHeading-sc-10oikoy-0"] {
			content: "kZQjgd,RtGqJ,"
		}

		/*!sc*/
		.fONQLM {
			border-width: 1px;
			border-color: hsla(216, 15%, 54%, 0.18);
			border-style: solid;
			background-color: hsla(216, 15%, 54%, 0.18);
			width: 100%;
			margin: 0;
		}

		/*!sc*/
		data-styled.g31[id="Divider__StyledDivider-sc-5tlrkc-0"] {
			content: "fONQLM,"
		}

		/*!sc*/
		.bRpweO {
			font-size: 40px;
		}

		/*!sc*/
		data-styled.g32[id="ContentPageHeading__StyledHeading-sc-1ojl0u5-0"] {
			content: "bRpweO,"
		}

		/*!sc*/
		.bzGFPE {
			cursor: pointer;
			padding: 8px;
			border-radius: 2px;
			background-color: transparent;
		}

		/*!sc*/
		.bzGFPE:hover {
			background-color: hsla(220, 30%, 96%, 1);
		}

		/*!sc*/
		@media (max-width:990px) {
			.bzGFPE:hover {
				background-color: hsla(216, 27%, 36%, 1);
			}
		}

		/*!sc*/
		data-styled.g33[id="styles__ColorSchemeChooserContainer-sc-1mkq7gc-0"] {
			content: "bzGFPE,"
		}

		/*!sc*/
		.gJSysE {
			background-color: hsla(213, 89%, 56%, 1);
			box-shadow: none;
			display: inline-block;
			cursor: pointer;
			border-width: 1px;
			border-style: solid;
			border-radius: 2px;
			border-color: hsla(213, 89%, 56%, 1);
			padding: 8px 12px 8px 12px;
		}

		/*!sc*/
		.gJSysE:hover {
			border-color: hsla(218, 89%, 51%, 1);
			background-color: hsla(218, 89%, 51%, 1);
		}

		/*!sc*/
		.gJSysE:active {
			border-color: hsla(227, 100%, 45%, 1);
			background-color: hsla(227, 100%, 45%, 1);
		}

		/*!sc*/
		.gJSysE:focus {
			border-color: hsla(223, 95%, 48%, 1);
			background-color: hsla(223, 95%, 48%, 1);
		}

		/*!sc*/
		.gJSysE:focus-visible {
			border-color: hsla(223, 95%, 48%, 1);
			background-color: hsla(223, 95%, 48%, 1);
		}

		/*!sc*/
		.gJSysE:focus-visible {
			border: 1px solid hsla(223, 95%, 48%, 1);
			background-color: hsla(223, 95%, 48%, 1);
		}

		/*!sc*/
		.gJSysE p {
			margin: 0;
		}

		/*!sc*/
		.czIuHx {
			background-color: transparent;
			box-shadow: none;
			display: inline-block;
			cursor: pointer;
			border-width: 1px;
			border-style: solid;
			border-radius: 2px;
			border-color: transparent;
			padding: 8px 12px 8px 12px;
		}

		/*!sc*/
		.czIuHx:hover {
			border-color: hsla(229, 12%, 45%, 1);
			background-color: hsla(231, 35%, 22%, 1);
		}

		/*!sc*/
		.czIuHx:active {
			border-color: hsla(229, 12%, 45%, 1);
			background-color: hsla(230, 23%, 29%, 1);
		}

		/*!sc*/
		.czIuHx:focus {
			border-color: hsla(229, 12%, 45%, 1);
			background-color: hsla(230, 23%, 29%, 1);
		}

		/*!sc*/
		.czIuHx:focus-visible {
			border-color: hsla(229, 12%, 45%, 1);
			background-color: hsla(230, 23%, 29%, 1);
		}

		/*!sc*/
		.czIuHx:focus-visible {
			border: 1px solid hsla(229, 12%, 45%, 1);
			background-color: hsla(230, 23%, 29%, 1);
		}

		/*!sc*/
		.czIuHx p {
			margin: 0;
		}

		/*!sc*/
		.rDRVp {
			background-color: transparent;
			box-shadow: none;
			display: inline-block;
			cursor: pointer;
			border-width: 1px;
			border-style: solid;
			border-radius: 2px;
			border-color: transparent;
			padding: 8px 12px 8px 12px;
		}

		/*!sc*/
		.rDRVp:hover {
			border-color: hsla(216, 19%, 89%, 1);
			background-color: hsla(220, 27%, 98%, 1);
		}

		/*!sc*/
		.rDRVp:active {
			border-color: hsla(216, 19%, 89%, 1);
			background-color: hsla(214, 21%, 94%, 1);
		}

		/*!sc*/
		.rDRVp:focus {
			border-color: hsla(216, 19%, 89%, 1);
			background-color: hsla(220, 30%, 96%, 1);
		}

		/*!sc*/
		.rDRVp:focus-visible {
			border-color: hsla(216, 19%, 89%, 1);
			background-color: hsla(220, 30%, 96%, 1);
		}

		/*!sc*/
		.rDRVp:focus-visible {
			border: 1px solid hsla(216, 19%, 89%, 1);
			background-color: hsla(220, 30%, 96%, 1);
		}

		/*!sc*/
		.rDRVp p {
			margin: 0;
		}

		/*!sc*/
		.fNlFXx {
			background-color: transparent;
			box-shadow: none;
			display: inline-block;
			cursor: pointer;
			border-width: 1px;
			border-style: solid;
			border-radius: 2px;
			border-color: transparent;
			padding: 8px;
		}

		/*!sc*/
		.fNlFXx:hover {
			border-color: hsla(216, 19%, 89%, 1);
			background-color: hsla(220, 27%, 98%, 1);
		}

		/*!sc*/
		.fNlFXx:active {
			border-color: hsla(216, 19%, 89%, 1);
			background-color: hsla(214, 21%, 94%, 1);
		}

		/*!sc*/
		.fNlFXx:focus {
			border-color: hsla(216, 19%, 89%, 1);
			background-color: hsla(220, 30%, 96%, 1);
		}

		/*!sc*/
		.fNlFXx:focus-visible {
			border-color: hsla(216, 19%, 89%, 1);
			background-color: hsla(220, 30%, 96%, 1);
		}

		/*!sc*/
		.fNlFXx:focus-visible {
			border: 1px solid hsla(216, 19%, 89%, 1);
			background-color: hsla(220, 30%, 96%, 1);
		}

		/*!sc*/
		.fNlFXx p {
			margin: 0;
		}

		/*!sc*/
		data-styled.g37[id="Button__StyledButton-sc-1g40twz-0"] {
			content: "gJSysE,czIuHx,rDRVp,fNlFXx,"
		}

		/*!sc*/
		.kpJmjg {
			color: hsla(0, 0%, 100%, 1);
		}

		/*!sc*/
		.imbcFy {
			color: inherit;
		}

		/*!sc*/
		data-styled.g38[id="Button__StyledText-sc-1g40twz-1"] {
			content: "kpJmjg,imbcFy,"
		}

		/*!sc*/
		.hSAbyp {
			border: none;
			background-color: inherit;
			border-radius: 4px;
			padding: 12px;
			margin: 0;
			padding-left: 48px;
			padding-right: 48px;
			font-family: Lato, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol";
			outline: none;
			-webkit-flex: 1;
			-ms-flex: 1;
			flex: 1;
			color: hsla(216, 27%, 36%, 1);
			position: relative;
		}

		/*!sc*/
		.hSAbyp:focus {
			border-color: hsla(223, 95%, 48%, 1);
		}

		/*!sc*/
		.hSAbyp::-webkit-input-placeholder {
			color: hsla(214, 18%, 69%, 1);
		}

		/*!sc*/
		.hSAbyp::-moz-placeholder {
			color: hsla(214, 18%, 69%, 1);
		}

		/*!sc*/
		.hSAbyp:-ms-input-placeholder {
			color: hsla(214, 18%, 69%, 1);
		}

		/*!sc*/
		.hSAbyp::placeholder {
			color: hsla(214, 18%, 69%, 1);
		}

		/*!sc*/
		.bxdbSG {
			border: none;
			background-color: inherit;
			border-radius: 0px;
			padding: 8px;
			margin: 0;
			padding-left: 16px;
			padding-right: 16px;
			font-family: Lato, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol";
			outline: none;
			-webkit-flex: 1;
			-ms-flex: 1;
			flex: 1;
			color: hsla(216, 27%, 36%, 1);
			position: relative;
		}

		/*!sc*/
		.bxdbSG:focus {
			border-color: hsla(223, 95%, 48%, 1);
		}

		/*!sc*/
		.bxdbSG::-webkit-input-placeholder {
			color: hsla(214, 18%, 69%, 1);
		}

		/*!sc*/
		.bxdbSG::-moz-placeholder {
			color: hsla(214, 18%, 69%, 1);
		}

		/*!sc*/
		.bxdbSG:-ms-input-placeholder {
			color: hsla(214, 18%, 69%, 1);
		}

		/*!sc*/
		.bxdbSG::placeholder {
			color: hsla(214, 18%, 69%, 1);
		}

		/*!sc*/
		data-styled.g41[id="Input__StyledInput-sc-1p8iijo-2"] {
			content: "hSAbyp,bxdbSG,"
		}

		/*!sc*/
		.iZtQst {
			border-color: hsla(216, 15%, 54%, 0.18);
			background: hsla(0, 0%, 100%, 1);
			margin: 0;
			font-family: Lato, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol";
			outline: none;
		}

		/*!sc*/
		.iZtQst:focus-within {
			border-color: hsla(223, 95%, 48%, 1);
		}

		/*!sc*/
		data-styled.g42[id="Input__StyledInputContainer-sc-1p8iijo-3"] {
			content: "iZtQst,"
		}

		/*!sc*/
		.cUcfME {
			position: absolute;
			left: 16px;
		}

		/*!sc*/
		.cUcfME path {
			fill: hsla(214, 18%, 69%, 1);
		}

		/*!sc*/
		data-styled.g43[id="Input__StyledIconLeft-sc-1p8iijo-4"] {
			content: "cUcfME,"
		}

		/*!sc*/
		.edKAZl {
			position: absolute;
			right: 16px;
		}

		/*!sc*/
		.edKAZl path {
			fill: hsla(214, 18%, 69%, 1);
		}

		/*!sc*/
		data-styled.g44[id="Input__StyledIconRight-sc-1p8iijo-5"] {
			content: "edKAZl,"
		}

		/*!sc*/
		.fTHyQm .Input__StyledButtonRight-sc-1p8iijo-1 {
			color: hsla(213, 89%, 56%, 1);
			min-height: 100%;
		}

		/*!sc*/
		data-styled.g45[id="DeveloperSubscription__StyledSubscriptionInput-sc-1gbefub-0"] {
			content: "fTHyQm,"
		}

		/*!sc*/
		.iAimGP {
			height: 2em;
		}

		/*!sc*/
		data-styled.g46[id="DeveloperSubscription__StyledErrorText-sc-1gbefub-1"] {
			content: "iAimGP,"
		}

		/*!sc*/
		.etdARH .Link__StyledLink-sc-38tiy-0:not(:last-child):after {
			content: '|';
			padding-right: 8px;
		}

		/*!sc*/
		data-styled.g47[id="Footer__FooterLinkContainer-sc-1snnb4l-0"] {
			content: "etdARH,"
		}

		/*!sc*/
		.ircWIJ {
			border: none;
			background-color: initial;
			-webkit-align-self: flex-end;
			-ms-flex-item-align: end;
			align-self: flex-end;
			visibility: hidden;
		}

		/*!sc*/
		.ircWIJ:hover {
			cursor: pointer;
		}

		/*!sc*/
		data-styled.g48[id="ScrollTop__StyledScrollTop-sc-1qkh247-0"] {
			content: "ircWIJ,"
		}

		/*!sc*/
		.gcQOFV {
			border: 1px solid hsla(216, 19%, 89%, 1);
			background-color: hsla(220, 30%, 96%, 1);
			border-radius: 50%;
		}

		/*!sc*/
		data-styled.g49[id="ScrollTop__StyledUpArrow-sc-1qkh247-1"] {
			content: "gcQOFV,"
		}

		/*!sc*/
		.hZUQuc {
			list-style: none;
			overflow-y: auto;
			padding-inline-start: 0px;
			margin-top: 8px;
			min-height: 250px;
		}

		/*!sc*/
		data-styled.g50[id="TableOfContents__ContentListContainer-sc-g0fs5p-0"] {
			content: "hZUQuc,"
		}

		/*!sc*/
		.gGzofQ {
			border-color: hsla(213, 89%, 56%, 1);
			border-left-width: 2px;
			-webkit-transition: border-left-width, border-color 100ms ease-in-out;
			transition: border-left-width, border-color 100ms ease-in-out;
		}

		/*!sc*/
		.ebOfVV {
			border-color: hsla(216, 19%, 89%, 1);
			border-left-width: 1;
			-webkit-transition: border-left-width, border-color 100ms ease-in-out;
			transition: border-left-width, border-color 100ms ease-in-out;
		}

		/*!sc*/
		data-styled.g51[id="TableOfContents__ContentListItem-sc-g0fs5p-1"] {
			content: "gGzofQ,ebOfVV,"
		}

		/*!sc*/
		.elEQwh {
			position: fixed;
			top: 0;
			left: 0;
			right: 0;
			bottom: 0;
			background: hsl(0, 0%, 0%, 0.7);
			padding: 0;
			overflow: auto;
		}

		/*!sc*/
		data-styled.g72[id="styled__StyledDialogOverlay-sc-7680y5-2"] {
			content: "elEQwh,"
		}

		/*!sc*/
		.gcqLlE {
			margin: 16px 0px;
			padding-left: 32px;
		}

		/*!sc*/
		data-styled.g98[id="styled__StyledUl-sc-hqnxju-1"] {
			content: "gcqLlE,"
		}

		/*!sc*/
		.jszEzM {
			vertical-align: top;
			color: hsla(216, 27%, 36%, 1);
			margin: 8px 0px;
		}

		/*!sc*/
		.jszEzM callout,
		.jszEzM .callout-container,
		.jszEzM ol,
		.jszEzM ul {
			margin: 8px 0px;
		}

		/*!sc*/
		.jszEzM callout li,
		.jszEzM .callout-container li,
		.jszEzM ol li,
		.jszEzM ul li {
			margin: 8px 0px;
		}

		/*!sc*/
		.jszEzM ol {
			margin-left: 12px;
		}

		/*!sc*/
		.jszEzM ol>li ol>li:before {
			content: counter(item, lower-roman) ".";
		}

		/*!sc*/
		.jszEzM ol>li:before {
			content: counter(item, lower-alpha) ".";
		}

		/*!sc*/
		.jszEzM ul {
			margin-left: 12px;
		}

		/*!sc*/
		.jszEzM img,
		.jszEzM video,
		.jszEzM iframe,
		.jszEzM .table-container {
			margin: 8px 0px;
		}

		/*!sc*/
		data-styled.g99[id="styled__StyledLi-sc-hqnxju-2"] {
			content: "jszEzM,"
		}

		/*!sc*/
		.dPWSDH {
			color: hsla(216, 27%, 36%, 1);
			font-size: 16px;
			line-height: 24px;
		}

		/*!sc*/
		.dPWSDH video {
			max-width: 100%;
		}

		/*!sc*/
		.dPWSDH iframe {
			height: 100%;
			width: 100%;
			max-width: 640px;
			aspect-ratio: 1.7;
		}

		/*!sc*/
		.dPWSDH .table-container {
			overflow-x: auto;
			overflow-y: clip;
		}

		/*!sc*/
		.dPWSDH .table-container .styled__StyledUl-sc-hqnxju-1 {
			padding-left: 24px;
		}

		/*!sc*/
		.dPWSDH .table-container .InlineCode__StyledInlineCode-sc-frpv5a-0,
		.dPWSDH .api-definition-container .InlineCode__StyledInlineCode-sc-frpv5a-0 {
			font-size: 12px;
			padding: 2px 4px;
			line-height: 20px;
		}

		/*!sc*/
		.dPWSDH h1,
		.dPWSDH h2,
		.dPWSDH h3,
		.dPWSDH h4 {
			color: hsla(217, 56%, 17%, 1);
			font-weight: 700;
			-webkit-scroll-margin-top: 56px;
			-moz-scroll-margin-top: 56px;
			-ms-scroll-margin-top: 56px;
			scroll-margin-top: 56px;
			margin-bottom: 12px;
		}

		/*!sc*/
		.dPWSDH h1 p,
		.dPWSDH h2 p,
		.dPWSDH h3 p,
		.dPWSDH h4 p {
			margin-top: 0px;
		}

		/*!sc*/
		.dPWSDH h1 {
			font-size: 28px;
			line-height: 40px;
			margin-top: 40px;
		}

		/*!sc*/
		.dPWSDH h2 {
			font-size: 24px;
			line-height: 40px;
			margin-top: 56px;
		}

		/*!sc*/
		.dPWSDH h3 {
			font-size: 20px;
			line-height: 28px;
			margin-top: 48px;
		}

		/*!sc*/
		.dPWSDH h4 {
			font-size: 18px;
			line-height: 28px;
			margin-top: 40px;
		}

		/*!sc*/
		.dPWSDH article:not(:last-child):after {
			content: '';
			display: block;
			padding-top: 40px;
			border-bottom: 1px solid #e6e6e6;
			margin-top: -1px;
		}

		/*!sc*/
		.dPWSDH article:not(:last-child).no-after {
			margin-top: 20px;
		}

		/*!sc*/
		.dPWSDH article:not(:last-child).no-after:after {
			margin-top: 0px;
		}

		/*!sc*/
		.dPWSDH p {
			margin: 16px 0;
			line-height: 24px;
		}

		/*!sc*/
		.dPWSDH a>p {
			margin: 0;
		}

		/*!sc*/
		.dPWSDH h1+p,
		.dPWSDH h2+p,
		.dPWSDH h3+p,
		.dPWSDH h4+p {
			margin-top: 0px;
		}

		/*!sc*/
		.dPWSDH img,
		.dPWSDH video,
		.dPWSDH iframe,
		.dPWSDH .table-container {
			margin-top: 16px;
		}

		/*!sc*/
		.dPWSDH li img,
		.dPWSDH p img,
		.dPWSDH li video,
		.dPWSDH p video,
		.dPWSDH li iframe,
		.dPWSDH p iframe,
		.dPWSDH li .table-container,
		.dPWSDH p .table-container {
			margin: 8px 0px;
		}

		/*!sc*/
		.dPWSDH ol,
		.dPWSDH ul {
			margin: 16px 0px;
		}

		/*!sc*/
		.dPWSDH li {
			margin: 8px 0px;
		}

		/*!sc*/
		.dPWSDH li callout,
		.dPWSDH li .callout-container,
		.dPWSDH li ol,
		.dPWSDH li ul {
			margin: 8px 0px;
		}

		/*!sc*/
		.dPWSDH li callout li,
		.dPWSDH li .callout-container li,
		.dPWSDH li ol li,
		.dPWSDH li ul li {
			margin: 8px 0px;
		}

		/*!sc*/
		.dPWSDH url,
		.dPWSDH .styled__ApiMethodContainer-sc-1jspfyw-0 {
			margin: 32px 0px;
		}

		/*!sc*/
		.dPWSDH aside,
		.dPWSDH pre {
			margin: 32px 0px;
		}

		/*!sc*/
		.dPWSDH url+aside,
		.dPWSDH url+pre,
		.dPWSDH .styled__ApiMethodContainer-sc-1jspfyw-0+.styled__CodeBlocksContainer-sc-hospau-1,
		.dPWSDH .styled__ApiMethodContainer-sc-1jspfyw-0+.styled__CodeBlockContainer-sc-hospau-6 {
			margin-top: -16px;
		}

		/*!sc*/
		.dPWSDH callout,
		.dPWSDH .callout-container {
			margin: 32px 0px;
		}

		/*!sc*/
		.dPWSDH .btn-new {
			display: block;
			-webkit-user-select: none;
			-moz-user-select: none;
			-ms-user-select: none;
			user-select: none;
			text-transform: none;
			cursor: pointer;
			border: 0;
			border-radius: 2px;
			-webkit-transition: .2s;
			transition: .2s;
			box-shadow: 0 3px 13px rgba(0, 0, 0, 0.09), 0 1px 5px 0 rgba(0, 0, 0, 0.14);
			margin: 16px 0;
			padding: 16px 20px;
			background: hsla(213, 89%, 56%, 1);
		}

		/*!sc*/
		.dPWSDH .btn-new:hover {
			background: hsla(218, 89%, 51%, 1);
		}

		/*!sc*/
		.dPWSDH .btn-new div:hover p,
		.dPWSDH .btn-new div:focus p,
		.dPWSDH .btn-new div:active p,
		.dPWSDH .btn-new a,
		.dPWSDH .btn-new p {
			font-weight: 700;
			color: hsla(0, 0%, 100%, 1);
		}

		/*!sc*/
		.dPWSDH .btn-new p {
			margin: 0px;
		}

		/*!sc*/
		data-styled.g100[id="styled__ContentContainer-sc-fg4p2w-0"] {
			content: "dPWSDH,"
		}

		/*!sc*/
		.HBTNX {
			cursor: pointer;
		}

		/*!sc*/
		data-styled.g101[id="Trigger__CollapsibleTrigger-sc-zrl3ha-0"] {
			content: "HBTNX,"
		}

		/*!sc*/
		.eWXbsW[data-state='open'] {
			-webkit-animation: eheAGG 300ms ease-out;
			animation: eheAGG 300ms ease-out;
			overflow: hidden;
			-webkit-animation-delay: -300ms;
			animation-delay: -300ms;
		}

		/*!sc*/
		.eWXbsW[data-state='closed'] {
			-webkit-animation: fDNIO 300ms ease-out;
			animation: fDNIO 300ms ease-out;
			overflow: hidden;
		}

		/*!sc*/
		data-styled.g102[id="Content__CollapsibleContent-sc-1bkq2us-0"] {
			content: "eWXbsW,"
		}

		/*!sc*/
		.fWgtQP a {
			width: 100%;
		}

		/*!sc*/
		data-styled.g103[id="SidebarNavLink__SidebarnavLinkContainer-sc-pt5di4-0"] {
			content: "fWgtQP,"
		}

		/*!sc*/
		.kVxEKo {
			color: hsla(216, 27%, 36%, 1);
		}

		/*!sc*/
		.kVxEKo:hover {
			color: hsla(217, 56%, 17%, 1);
		}

		/*!sc*/
		.kkEfVJ {
			color: hsla(213, 89%, 56%, 1);
			false;
		}

		/*!sc*/
		data-styled.g104[id="SidebarNavLink__SidebarnavLinkText-sc-pt5di4-1"] {
			content: "kVxEKo,kkEfVJ,"
		}

		/*!sc*/
		.jVrtuA {
			border-left: 1px solid hsla(216, 19%, 89%, 1);
		}

		/*!sc*/
		data-styled.g105[id="NavigationTree__NavNodesContainer-sc-1f9wbbd-0"] {
			content: "jVrtuA,"
		}

		/*!sc*/
		.bktzmf {
			false border-radius: 2px;
			margin-bottom: 4px;
		}

		/*!sc*/
		.iZcbJV {
			background-color: hsla(216, 15%, 54%, 0.09);
			border-radius: 2px;
			margin-bottom: 4px;
		}

		/*!sc*/
		data-styled.g106[id="NavigationTree__StyledFlex-sc-1f9wbbd-1"] {
			content: "bktzmf,iZcbJV,"
		}

		/*!sc*/
		.coZHyU {
			color: hsla(216, 27%, 36%, 1);
		}

		/*!sc*/
		.coZHyU:hover {
			color: hsla(217, 56%, 17%, 1);
		}

		/*!sc*/
		.hGeEcs {
			color: hsla(217, 56%, 17%, 1);
		}

		/*!sc*/
		.hGeEcs:hover {
			color: hsla(217, 56%, 17%, 1);
		}

		/*!sc*/
		.gknCtx {
			color: hsla(217, 18%, 45%, 1);
		}

		/*!sc*/
		.gknCtx:hover {
			color: hsla(216, 27%, 36%, 1);
		}

		/*!sc*/
		data-styled.g107[id="NavigationTree__NavNodeCollapsibleTriggerText-sc-1f9wbbd-2"] {
			content: "coZHyU,hGeEcs,gknCtx,"
		}

		/*!sc*/
		.bOsaqT {
			position: relative;
		}

		/*!sc*/
		.bOsaqT:hover {
			background: hsla(218, 89%, 51%, 0.09);
		}

		/*!sc*/
		.bOsaqT:before {
			content: '';
			position: absolute;
			width: 4px;
			height: 100%;
			box-shadow: 2px 0px 2px rgba(0, 0, 0, 0.08);
		}

		/*!sc*/
		.vKhFP {
			position: relative;
			background: linear-gradient(180deg, hsla(213, 89%, 56%, 1) 0%, hsla(218, 89%, 51%, 1) 100%);
			box-shadow: 0px 3px 8px rgba(21, 45, 75, 0.2), 0px 0px 1px rgba(21, 45, 75, 0.2);
		}

		/*!sc*/
		.vKhFP:before {
			content: '';
			position: absolute;
			width: 4px;
			height: 100%;
			background: hsla(223, 95%, 48%, 1);
			box-shadow: 2px 0px 2px rgba(0, 0, 0, 0.08);
		}

		/*!sc*/
		data-styled.g108[id="RootNavigationBar__RootNavItemWrapper-sc-1tris5i-0"] {
			content: "bOsaqT,vKhFP,"
		}

		/*!sc*/
		.VRnDM {
			border-right: 1px solid hsla(216, 15%, 54%, 0.18);
		}

		/*!sc*/
		data-styled.g110[id="RootNavigationBar__RootNavContainer-sc-1tris5i-2"] {
			content: "VRnDM,"
		}

		/*!sc*/
		.jDohtf .Button__StyledText-sc-1g40twz-1 {
			color: hsla(0, 0%, 100%, 1);
		}

		/*!sc*/
		data-styled.g111[id="CallToAction__CallToActionContainer-sc-fywsk9-0"] {
			content: "jDohtf,"
		}

		/*!sc*/
		.jFnfpE {
			display: block;
			width: 100%;
			aspect-ratio: 6.09375;
			height: 100%;
			max-width: 100%;
			max-height: 100%;
			object-fit: contain;
		}

		/*!sc*/
		.lbdtLD {
			display: block;
			width: 100%;
			aspect-ratio: 4.375;
			height: 100%;
			max-width: 100%;
			max-height: 100%;
			object-fit: contain;
		}

		/*!sc*/
		data-styled.g113[id="styled__StyledImage-sc-jbtw7r-1"] {
			content: "jFnfpE,lbdtLD,"
		}

		/*!sc*/
		.eQWLvM .Input__StyledInput-sc-1p8iijo-2 {
			box-sizing: border-box;
			max-width: 100%;
			background-color: hsla(220, 27%, 98%, 1);
		}

		/*!sc*/
		.eQWLvM .Input__StyledIconRight-sc-1p8iijo-5 {
			display: none;
		}

		/*!sc*/
		@media (any-pointer:fine) {
			.eQWLvM .Input__StyledIconRight-sc-1p8iijo-5 {
				display: block;
			}
		}

		/*!sc*/
		data-styled.g124[id="Search__StyledSearch-sc-m3uzep-0"] {
			content: "eQWLvM,"
		}

		/*!sc*/
		.fCXonT .Link__StyledText-sc-38tiy-2 {
			font-weight: 400;
			color: hsla(216, 27%, 36%, 1);
		}

		/*!sc*/
		.Link__StyledLink-sc-38tiy-0:hover .NavLink__StyledNavLink-sc-ni1far-0 .Link__StyledText-sc-38tiy-2 {
			color: hsla(213, 89%, 56%, 1);
		}

		/*!sc*/
		.Link__StyledLink-sc-38tiy-0:focus .NavLink__StyledNavLink-sc-ni1far-0 .Link__StyledText-sc-38tiy-2 {
			color: hsla(213, 89%, 56%, 1);
		}

		/*!sc*/
		data-styled.g125[id="NavLink__StyledNavLink-sc-ni1far-0"] {
			content: "fCXonT,"
		}

		/*!sc*/
		.dICFTk {
			border-bottom: 1px solid hsla(216, 15%, 54%, 0.18);
		}

		/*!sc*/
		data-styled.g129[id="DesktopHeader__StyledHeader-sc-1ho5vft-0"] {
			content: "dICFTk,"
		}

		/*!sc*/
		.dvfyQb {
			background-image: url(/docs/build/browser/static/header-background-mobile.c6c08fad.png);
			background-repeat: no-repeat;
			background-size: cover;
			width: 100%;
			height: 100%;
		}

		/*!sc*/
		data-styled.g130[id="BackgroundImage__StyledBackgroundImage-sc-ur9uoe-0"] {
			content: "dvfyQb,"
		}

		/*!sc*/
		.zTWgS {
			position: -webkit-sticky;
			position: sticky;
			top: 0;
			z-index: 2;
		}

		/*!sc*/
		data-styled.g131[id="Header__HeaderNav-sc-13q5qca-0"] {
			content: "zTWgS,"
		}

		/*!sc*/
		.ggcwSt {
			display: inline;
			color: hsla(217, 56%, 17%, 1);
			font-size: 28px;
			line-height: 40px;
			font-weight: 700;
		}

		/*!sc*/
		data-styled.g133[id="styled__StyledHeadingText-sc-c6l8fk-1"] {
			content: "ggcwSt,"
		}

		/*!sc*/
		.jITCZt {
			display: none;
		}

		/*!sc*/
		.jITCZt path {
			fill: hsla(213, 89%, 56%, 1);
		}

		/*!sc*/
		.styled__StyledLink-sc-c6l8fk-0:hover .styled__StyledHeadingIcon-sc-c6l8fk-2 {
			display: inline;
		}

		/*!sc*/
		data-styled.g134[id="styled__StyledHeadingIcon-sc-c6l8fk-2"] {
			content: "jITCZt,"
		}

		/*!sc*/
		.eEHZvo {
			margin: revert;
			line-height: 24px;
		}

		/*!sc*/
		data-styled.g135[id="Text__StyledTextComponent-sc-16y34hf-0"] {
			content: "eEHZvo,"
		}

		/*!sc*/
		.chZHUd p,
		li .chZHUd {
			display: inline;
		}

		/*!sc*/
		.chZHUd .Link__StyledText-sc-38tiy-2,
		.chZHUd strong,
		.chZHUd em {
			display: inline;
		}

		/*!sc*/
		.chZHUd a,
		.chZHUd strong,
		.chZHUd em {
			color: hsla(213, 89%, 56%, 1);
		}

		/*!sc*/
		.chZHUd:hover {
			color: hsla(218, 89%, 51%, 1);
		}

		/*!sc*/
		.chZHUd:hover a,
		.chZHUd:hover strong,
		.chZHUd:hover em {
			color: hsla(218, 89%, 51%, 1);
		}

		/*!sc*/
		.chZHUd:focus {
			color: hsla(223, 95%, 48%, 1);
		}

		/*!sc*/
		.chZHUd:focus a,
		.chZHUd:focus strong,
		.chZHUd:focus em {
			color: hsla(223, 95%, 48%, 1);
		}

		/*!sc*/
		.chZHUd:active {
			color: hsla(223, 95%, 48%, 1);
		}

		/*!sc*/
		.chZHUd:active a,
		.chZHUd:active strong,
		.chZHUd:active em {
			color: hsla(223, 95%, 48%, 1);
		}

		/*!sc*/
		data-styled.g136[id="styled__StyledContentLink-sc-r9g6hi-0"] {
			content: "chZHUd,"
		}

		/*!sc*/
		.emxFrX {
			padding: 4px 16px;
			background-color: hsla(155, 100%, 31%, 0.09);
			border-width: 1px;
			border-radius: 0px;
			border-style: solid;
			border-color: hsla(155, 100%, 31%, 0.32);
		}

		/*!sc*/
		@media screen and (min-width:550px) {
			.emxFrX {
				padding: 4px 20px;
			}
		}

		/*!sc*/
		.emxFrX .Button__StyledText-sc-1g40twz-1 {
			color: hsla(160, 100%, 26%, 1);
		}

		/*!sc*/
		data-styled.g150[id="styles__PositiveFeedbackButton-sc-1ahuhrc-0"] {
			content: "emxFrX,"
		}

		/*!sc*/
		.etjtqK {
			padding: 4px 20px;
			background-color: hsla(9, 91%, 56%, 0.09);
			border-width: 1px;
			border-radius: 0px;
			border-style: solid;
			border-color: hsla(9, 91%, 56%, 0.32);
		}

		/*!sc*/
		.etjtqK .Button__StyledText-sc-1g40twz-1 {
			color: hsla(8, 73%, 47%, 1);
		}

		/*!sc*/
		data-styled.g151[id="styles__NegativeFeedbackButton-sc-1ahuhrc-1"] {
			content: "etjtqK,"
		}

		/*!sc*/
		html,
		body {
			width: 100%;
			height: 100%;
			font-family: Lato, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol";
			-webkit-scroll-behavior: smooth;
			-moz-scroll-behavior: smooth;
			-ms-scroll-behavior: smooth;
			scroll-behavior: smooth;
		}

		/*!sc*/
		body {
			box-sizing: border-box;
			margin: 0;
			padding: 0;
		}

		/*!sc*/
		#root {
			min-height: 100%;
			isolation: isolate;
		}

		/*!sc*/
		figure {
			margin: 0;
			padding: 0;
		}

		/*!sc*/
		data-styled.g174[id="sc-global-bvpwpj1"] {
			content: "sc-global-bvpwpj1,"
		}

		/*!sc*/
		@-webkit-keyframes eheAGG {
			0% {
				height: 0;
				opacity: 0;
			}

			100% {
				height: var(--radix-collapsible-content-height);
				opacity: 1;
			}
		}

		/*!sc*/
		@keyframes eheAGG {
			0% {
				height: 0;
				opacity: 0;
			}

			100% {
				height: var(--radix-collapsible-content-height);
				opacity: 1;
			}
		}

		/*!sc*/
		data-styled.g190[id="sc-keyframes-eheAGG"] {
			content: "eheAGG,"
		}

		/*!sc*/
		@-webkit-keyframes fDNIO {
			0% {
				height: var(--radix-collapsible-content-height);
				opacity: 1;
			}

			100% {
				height: 0;
				opacity: 0;
			}
		}

		/*!sc*/
		@keyframes fDNIO {
			0% {
				height: var(--radix-collapsible-content-height);
				opacity: 1;
			}

			100% {
				height: 0;
				opacity: 0;
			}
		}

		/*!sc*/
		data-styled.g191[id="sc-keyframes-fDNIO"] {
			content: "fDNIO,"
		}

		/*!sc*/
	</style>
</head>

<body>
	<div id="root">
		<div class="Box-sc-5vx4ls-0 hHKSeB">
			<nav class="Box-sc-5vx4ls-0 Header__HeaderNav-sc-13q5qca-0 cGOgLs zTWgS">
				<div display="[object Object]" height="56" width="100%"
					class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 lisYMx bNqftg DesktopHeader__StyledHeader-sc-1ho5vft-0 dICFTk">
					<div display="flex" class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 hFpJwV fCPAWO">
						<div display="flex" width="195" height="32"
							class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 YlgZr fCPAWO Link__StyledLink-sc-38tiy-0 kWnpZi">
							<a target="_self" href="/docs/">
								<div class="Box-sc-5vx4ls-0 gHBrCZ">
									<img alt="Razorpay Docs Logo" src="/docs/build/browser/static/razorpay-docs-dark.6f09b030.svg" width="195" height="32" loading="eager" class="styled__StyledImage-sc-jbtw7r-1 jFnfpE"/></div>
							</a></div>
						<div display="flex" width="fit-content" tabindex="0"
							class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 bHbUpq jcarLi Input__StyledInputContainer-sc-1p8iijo-3 iZtQst Search__StyledSearch-sc-m3uzep-0 eQWLvM">
							<input placeholder="Search the documentation" disabled="" value="" tabindex="0" class="Input__StyledInput-sc-1p8iijo-2 hSAbyp Search__StyledSearch-sc-m3uzep-0 eQWLvM"/><svg
								width="20" height="20" viewBox="0 0 16 16" fill="none"
								xmlns="http://www.w3.org/2000/svg" class="Input__StyledIconLeft-sc-1p8iijo-4 cUcfME">
								<path fill-rule="evenodd" clip-rule="evenodd"
									d="M7.19999 0C3.22355 0 0 3.22355 0 7.19999C0 11.1764 3.22355 14.4 7.19999 14.4C8.9 14.4 10.4624 13.8108 11.6941 12.8255L14.6343 15.7657C14.9467 16.0781 15.4533 16.0781 15.7657 15.7657C16.0781 15.4533 16.0781 14.9467 15.7657 14.6343L12.8255 11.6941C13.8108 10.4624 14.4 8.9 14.4 7.19999C14.4 3.22355 11.1764 0 7.19999 0ZM11.233 11.0852C12.2033 10.0783 12.8 8.70881 12.8 7.19999C12.8 4.1072 10.2928 1.6 7.19999 1.6C4.1072 1.6 1.6 4.1072 1.6 7.19999C1.6 10.2928 4.1072 12.8 7.19999 12.8C8.70881 12.8 10.0783 12.2033 11.0852 11.233C11.1063 11.2056 11.1293 11.1794 11.1543 11.1543C11.1794 11.1293 11.2056 11.1063 11.233 11.0852Z"
									fill="#132644"></path>
							</svg>
							<div data-blade-component="box" display="flex"
								class="BaseBoxweb__BaseBox-sc-1icfu8j-0 dCZIGP">
								<div width="20" height="20"
									class="SearchRight__SearchRightContainer-sc-9nccfz-0 bRSBxk"><span>/</span></div>
							</div>
						</div>
					</div>
					<div display="flex" height="32" class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 fiVOLr kNUFIs">
						<div class="Box-sc-5vx4ls-0 ddVbIH">
							<div display="flex" role="button" aria-label="change color scheme"
								class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 dPVYbu fCPAWO styles__ColorSchemeChooserContainer-sc-1mkq7gc-0 bzGFPE">
								<svg aria-hidden="true" data-blade-component="icon" height="20px" viewBox="0 0 24 24"
									width="20px" fill="none" data-testid="light-mode"
									class="Svgweb__StyledSvg-vcmjs8-0">
									<g clip-path="url(#clip0_60_388)">
										<path
											d="M6 12C6 8.68629 8.68629 6 12 6C15.3137 6 18 8.68629 18 12C18 15.3137 15.3137 18 12 18C8.68629 18 6 15.3137 6 12ZM12 8C9.79086 8 8 9.79086 8 12C8 14.2091 9.79086 16 12 16C14.2091 16 16 14.2091 16 12C16 9.79086 14.2091 8 12 8Z"
											clip-rule="evenodd" fill="hsla(216, 16%, 60%, 1)" fill-rule="evenodd">
										</path>
										<path
											d="M12 0C12.5523 0 13 0.447715 13 1V3C13 3.55228 12.5523 4 12 4C11.4477 4 11 3.55228 11 3V1C11 0.447715 11.4477 0 12 0Z"
											clip-rule="evenodd" fill="hsla(216, 16%, 60%, 1)" fill-rule="evenodd">
										</path>
										<path
											d="M12 20C12.5523 20 13 20.4477 13 21V23C13 23.5523 12.5523 24 12 24C11.4477 24 11 23.5523 11 23V21C11 20.4477 11.4477 20 12 20Z"
											clip-rule="evenodd" fill="hsla(216, 16%, 60%, 1)" fill-rule="evenodd">
										</path>
										<path
											d="M3.51289 3.51289C3.90342 3.12237 4.53658 3.12237 4.92711 3.51289L6.34711 4.93289C6.73763 5.32342 6.73763 5.95658 6.34711 6.34711C5.95658 6.73763 5.32342 6.73763 4.93289 6.34711L3.51289 4.92711C3.12237 4.53658 3.12237 3.90342 3.51289 3.51289Z"
											clip-rule="evenodd" fill="hsla(216, 16%, 60%, 1)" fill-rule="evenodd">
										</path>
										<path
											d="M17.6529 17.6529C18.0434 17.2624 18.6766 17.2624 19.0671 17.6529L20.4871 19.0729C20.8776 19.4634 20.8776 20.0966 20.4871 20.4871C20.0966 20.8776 19.4634 20.8776 19.0729 20.4871L17.6529 19.0671C17.2624 18.6766 17.2624 18.0434 17.6529 17.6529Z"
											clip-rule="evenodd" fill="hsla(216, 16%, 60%, 1)" fill-rule="evenodd">
										</path>
										<path
											d="M0 12C0 11.4477 0.447715 11 1 11H3C3.55228 11 4 11.4477 4 12C4 12.5523 3.55228 13 3 13H1C0.447715 13 0 12.5523 0 12Z"
											clip-rule="evenodd" fill="hsla(216, 16%, 60%, 1)" fill-rule="evenodd">
										</path>
										<path
											d="M20 12C20 11.4477 20.4477 11 21 11H23C23.5523 11 24 11.4477 24 12C24 12.5523 23.5523 13 23 13H21C20.4477 13 20 12.5523 20 12Z"
											clip-rule="evenodd" fill="hsla(216, 16%, 60%, 1)" fill-rule="evenodd">
										</path>
										<path
											d="M6.34711 17.6529C6.73763 18.0434 6.73763 18.6766 6.34711 19.0671L4.92711 20.4871C4.53658 20.8776 3.90342 20.8776 3.51289 20.4871C3.12237 20.0966 3.12237 19.4634 3.51289 19.0729L4.93289 17.6529C5.32342 17.2624 5.95658 17.2624 6.34711 17.6529Z"
											clip-rule="evenodd" fill="hsla(216, 16%, 60%, 1)" fill-rule="evenodd">
										</path>
										<path
											d="M20.4871 3.51289C20.8776 3.90342 20.8776 4.53658 20.4871 4.92711L19.0671 6.34711C18.6766 6.73763 18.0434 6.73763 17.6529 6.34711C17.2624 5.95658 17.2624 5.32342 17.6529 4.93289L19.0729 3.51289C19.4634 3.12237 20.0966 3.12237 20.4871 3.51289Z"
											clip-rule="evenodd" fill="hsla(216, 16%, 60%, 1)" fill-rule="evenodd">
										</path>
									</g>
									<defs>
										<clipPath id="clip0_60_388">
											<rect height="24" width="24" fill="hsla(216, 16%, 60%, 1)"></rect>
										</clipPath>
									</defs>
								</svg></div>
						</div>
						<div display="flex" height="24"
							class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 gIjuDY foqTwv">
							<div class="Box-sc-5vx4ls-0 NavLink__StyledNavLink-sc-ni1far-0 cGOgLs fCXonT">
								<div display="flex"
									class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 dPVYbu fCPAWO Link__StyledLink-sc-38tiy-0 kWnpZi">
									<a href="https://razorpay.com/pricing/" target="_blank" rel="noopener noreferrer">
										<p class="Text-sc-1g8cvhx-0 Link__StyledText-sc-38tiy-2 jyrMiD fLetpi">Pricing
										</p>
									</a></div>
							</div>
							<div class="Box-sc-5vx4ls-0 NavLink__StyledNavLink-sc-ni1far-0 cGOgLs fCXonT">
								<div display="flex"
									class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 dPVYbu fCPAWO Link__StyledLink-sc-38tiy-0 kWnpZi">
									<a target="_self" href="/docs/api">
										<p class="Text-sc-1g8cvhx-0 Link__StyledText-sc-38tiy-2 jyrMiD fLetpi">API
											Reference</p>
									</a></div>
							</div>
							<div class="Box-sc-5vx4ls-0 NavLink__StyledNavLink-sc-ni1far-0 cGOgLs fCXonT">
								<div display="flex"
									class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 dPVYbu fCPAWO Link__StyledLink-sc-38tiy-0 kWnpZi">
									<a href="https://razorpay.com/support/" target="_blank" rel="noopener noreferrer">
										<p class="Text-sc-1g8cvhx-0 Link__StyledText-sc-38tiy-2 jyrMiD fLetpi">Support
										</p>
									</a></div>
							</div>
						</div>
						<div display="flex" class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 dPVYbu fCPAWO">
							<div display="flex" height="24"
								class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 jObrhw fCPAWO Link__StyledLink-sc-38tiy-0 kWnpZi">
								<a href="https://dashboard.razorpay.com/?next=%2Fdocs%2F%2Fpayments%2Fpayment-gateway%2Fecommerce-plugins#/access/signin"
									target="_self" rel="noopener noreferrer">
									<p class="Text-sc-1g8cvhx-0 Link__StyledText-sc-38tiy-2 kgsGEf fLetpi">Log In</p>
								</a></div>
							<div display="flex"
								class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 dPVYbu fCPAWO Link__StyledLink-sc-38tiy-0 kWnpZi">
								<a href="https://dashboard.razorpay.com/signup" target="_self"
									rel="noopener noreferrer"><button role="link" class="Button__StyledButton-sc-1g40twz-0 gJSysE CallToAction__CallToActionContainer-sc-fywsk9-0 jDohtf"><p class="Text-sc-1g8cvhx-0 Button__StyledText-sc-1g40twz-1 HSevc kpJmjg">Sign Up</p></button></a>
							</div>
						</div>
					</div>
				</div>
				<div display="[object Object]" class="Box-sc-5vx4ls-0 dWwBrM">
					<div class="Box-sc-5vx4ls-0 cGOgLs">
						<div class="Box-sc-5vx4ls-0 BackgroundImage__StyledBackgroundImage-sc-ur9uoe-0 cGOgLs dvfyQb">
							<div display="flex" height="56" width="100%"
								class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 fMFaKg ldIsSH">
								<div display="flex" height="32"
									class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 fiVOLr ekisLk">
									<div display="flex" width="140" height="32"
										class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 btLJLX fCPAWO Link__StyledLink-sc-38tiy-0 kWnpZi">
										<a target="_self" href="/docs/">
											<div class="Box-sc-5vx4ls-0 veVFF">
												<img alt="Razorpay Docs Logo" src="/docs/build/browser/static/razorpay-docs-light.009264f2.svg" width="140" height="32" loading="eager" class="styled__StyledImage-sc-jbtw7r-1 lbdtLD"/></div>
										</a></div>
								</div>
								<div display="flex" class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 dPVYbu gbpuuV">
									<div display="flex" height="32"
										class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 jAGyDA fCPAWO">
										<button class="Button__StyledButton-sc-1g40twz-0 czIuHx"><svg width="24" height="24" viewBox="0 0 20 14" fill="none" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" clip-rule="evenodd" d="M0 7C0 6.44772 0.447715 6 1 6H19C19.5523 6 20 6.44772 20 7C20 7.55228 19.5523 8 19 8H1C0.447715 8 0 7.55228 0 7Z" fill="#ffffff"></path><path fill-rule="evenodd" clip-rule="evenodd" d="M0 1C0 0.447715 0.447715 0 1 0H19C19.5523 0 20 0.447715 20 1C20 1.55228 19.5523 2 19 2H1C0.447715 2 0 1.55228 0 1Z" fill="#ffffff"></path><path fill-rule="evenodd" clip-rule="evenodd" d="M0 13C0 12.4477 0.447715 12 1 12H19C19.5523 12 20 12.4477 20 13C20 13.5523 19.5523 14 19 14H1C0.447715 14 0 13.5523 0 13Z" fill="#ffffff"></path></svg></button>
									</div>
								</div>
							</div>
						</div>
					</div>
				</div>
			</nav>
			<div display="flex" width="100%" class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 bgUKhf gbpuuV">
				<div display="[object Object]" width="fit-content" height="calc(100vh - 56px)"
					class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 ixGcEy gbpuuV">
					<nav width="72" display="[object Object]"
						class="Box-sc-5vx4ls-0 RootNavigationBar__RootNavContainer-sc-1tris5i-2 ctYFNB VRnDM">
						<div class="Box-sc-5vx4ls-0 RootNavigationBar__RootNavItemWrapper-sc-1tris5i-0 cGOgLs bOsaqT">
							<div display="flex"
								class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 dPVYbu fCPAWO Link__StyledLink-sc-38tiy-0 kWnpZi">
								<a target="_self"
									href="/docs/"><span display="flex" width="72" height="72" class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 dLhSPJ enkULn"><svg width="16" height="16" viewBox="0 0 14 15" fill="none" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" clip-rule="evenodd" d="M7.39253 0.912591C7.16142 0.732831 6.8378 0.732831 6.60668 0.912591L0.846685 5.39259C0.690792 5.51384 0.599609 5.70028 0.599609 5.89777V12.9378C0.599609 13.9981 1.45922 14.8578 2.51961 14.8578H11.4796C12.54 14.8578 13.3996 13.9981 13.3996 12.9378V5.89777C13.3996 5.70028 13.3084 5.51384 13.1525 5.39259L7.39253 0.912591ZM9.55962 13.5778H11.4796C11.833 13.5778 12.1196 13.2912 12.1196 12.9378V6.21079L6.99961 2.22856L1.87961 6.21079V12.9378C1.87961 13.2912 2.16614 13.5778 2.51961 13.5778H4.43961V7.81777C4.43961 7.46431 4.72614 7.17777 5.07961 7.17777H8.91962C9.27304 7.17777 9.55962 7.46431 9.55962 7.81777V13.5778ZM5.71961 13.5778V8.45777H8.27962V13.5778H5.71961Z" fill="#FFF" stroke="#FFF" stroke-width="0"></path></svg><span class="Text-sc-1g8cvhx-0 cmLnxL">Home</span></span></a>
							</div>
						</div>
						<div class="Box-sc-5vx4ls-0 RootNavigationBar__RootNavItemWrapper-sc-1tris5i-0 cGOgLs bOsaqT">
							<div display="flex"
								class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 dPVYbu fCPAWO Link__StyledLink-sc-38tiy-0 kWnpZi">
								<a target="_self"
									href="/docs/get-started"><span display="flex" width="72" height="72" class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 dLhSPJ enkULn"><svg width="16" height="16" viewBox="0 0 14 14" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M8.40616 13C8.25762 13.0014 8.11163 12.9614 7.98456 12.8844C7.8575 12.8075 7.75439 12.6966 7.68681 12.5644L6.08826 9.53911C6.0419 9.44561 6.03395 9.33768 6.06612 9.23839C6.09829 9.1391 6.16803 9.05634 6.26042 9.0078C6.35281 8.95926 6.46052 8.94878 6.56054 8.97861C6.66055 9.00845 6.74492 9.07622 6.79562 9.16745L8.39417 12.1927L12.2147 1.83411L1.82414 5.60269L5.74058 7.70478L9.06556 4.3798C9.14081 4.30455 9.24287 4.26227 9.3493 4.26227C9.45572 4.26227 9.55779 4.30455 9.63304 4.3798C9.70829 4.45505 9.75057 4.55712 9.75057 4.66354C9.75057 4.76997 9.70829 4.87203 9.63304 4.94728L6.09625 8.48007C6.03613 8.54028 5.95835 8.57972 5.87426 8.59266C5.79016 8.6056 5.70412 8.59136 5.62868 8.55201L1.46047 6.33802C1.31457 6.26974 1.19271 6.15896 1.11086 6.02022C1.02901 5.88147 0.990998 5.72124 1.0018 5.56051C1.0126 5.39979 1.07171 5.24608 1.17139 5.11954C1.27107 4.99299 1.40665 4.89952 1.56038 4.85137L11.915 1.06281C12.0614 1.00105 12.223 0.984352 12.379 1.01486C12.535 1.04537 12.6783 1.12171 12.7907 1.2341C12.9031 1.3465 12.9795 1.48986 13.01 1.64585C13.0405 1.80185 13.0238 1.9634 12.962 2.10986L9.17346 12.4645C9.12137 12.6142 9.02593 12.7451 8.89926 12.8404C8.77259 12.9358 8.62042 12.9913 8.46211 13H8.40616Z" fill="#FFF" stroke="#FFF" stroke-width="0.3"></path></svg><span class="Text-sc-1g8cvhx-0 cmLnxL">Get Started</span></span></a>
							</div>
						</div>
						<div class="Box-sc-5vx4ls-0 RootNavigationBar__RootNavItemWrapper-sc-1tris5i-0 cGOgLs vKhFP">
							<div display="flex"
								class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 dPVYbu fCPAWO Link__StyledLink-sc-38tiy-0 kWnpZi">
								<a target="_self"
									href="/docs/payments"><span display="flex" width="72" height="72" class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 dLhSPJ enkULn"><svg width="16" height="16" viewBox="0 0 14 11" fill="none" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" clip-rule="evenodd" d="M12.333 0.333344H1.66634C0.926341 0.333344 0.339675 0.926677 0.339675 1.66668L0.333008 9.66668C0.333008 10.4067 0.926341 11 1.66634 11H12.333C13.073 11 13.6663 10.4067 13.6663 9.66668V1.66668C13.6663 0.926677 13.073 0.333344 12.333 0.333344ZM12.333 9.66668H1.66634V5.66668H12.333V9.66668ZM12.333 4.33334H1.66634V1.66668H12.333V4.33334ZM11.8886 7.44445C11.8886 7.93539 11.4906 8.33334 10.9997 8.33334C10.5087 8.33334 10.1108 7.93539 10.1108 7.44445C10.1108 6.95352 10.5087 6.55557 10.9997 6.55557C11.4906 6.55557 11.8886 6.95352 11.8886 7.44445ZM10.1108 7.44445C10.1108 6.95352 9.71283 6.55557 9.2219 6.55557C8.73096 6.55557 8.33301 6.95352 8.33301 7.44445C8.33301 7.93539 8.73096 8.33334 9.2219 8.33334C9.71283 8.33334 10.1108 7.93539 10.1108 7.44445Z" fill="#FFF"></path></svg><span class="Text-sc-1g8cvhx-0 cmLnxL">Payments</span></span></a>
							</div>
						</div>
						<div class="Box-sc-5vx4ls-0 RootNavigationBar__RootNavItemWrapper-sc-1tris5i-0 cGOgLs bOsaqT">
							<div display="flex"
								class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 dPVYbu fCPAWO Link__StyledLink-sc-38tiy-0 kWnpZi">
								<a target="_self"
									href="/docs/x"><span display="flex" width="72" height="72" class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 dLhSPJ enkULn"><svg width="16" height="16" viewBox="0 0 14 16" fill="none" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" clip-rule="evenodd" d="M11.5696 5.48906H2.39501L6.99402 2.19613L11.5696 5.48906ZM1.01893 4.86659L6.23301 1.13327C6.68899 0.806786 7.30242 0.807529 7.75761 1.13512L12.9419 4.86614C13.2201 5.06634 13.385 5.38814 13.385 5.73088C13.385 6.31928 12.908 6.79628 12.3195 6.79628H1.63854C1.05073 6.79628 0.574219 6.31976 0.574219 5.73196C0.574219 5.38866 0.73981 5.06645 1.01893 4.86659ZM1.92272 8.94109C1.92272 8.50884 2.27311 8.15844 2.70533 8.15844C3.13755 8.15844 3.48794 8.50884 3.48794 8.94109V12.0956C3.48794 12.5278 3.13755 12.8782 2.70533 12.8782C2.27311 12.8782 1.92272 12.5278 1.92272 12.0956V8.94109ZM6.1643 8.97372C6.1643 8.52347 6.52932 8.15844 6.97959 8.15844C7.42986 8.15844 7.79488 8.52347 7.79488 8.97372V12.0629C7.79488 12.5132 7.42986 12.8782 6.97959 12.8782C6.52932 12.8782 6.1643 12.5132 6.1643 12.0629V8.97372ZM1.25879 15.5958C0.880708 15.5958 0.574219 15.2894 0.574219 14.9112C0.574219 14.5332 0.880708 14.2267 1.25879 14.2267H12.7004C13.0785 14.2267 13.385 14.5332 13.385 14.9112C13.385 15.2894 13.0785 15.5958 12.7004 15.5958H1.25879ZM10.4713 8.94109C10.4713 8.50884 10.8217 8.15844 11.2538 8.15844C11.6861 8.15844 12.0364 8.50884 12.0364 8.94109V12.0956C12.0364 12.5278 11.6861 12.8782 11.2538 12.8782C10.8217 12.8782 10.4713 12.5278 10.4713 12.0956V8.94109Z" fill="#FFF"></path></svg><span class="Text-sc-1g8cvhx-0 cmLnxL">Banking Plus</span></span></a>
							</div>
						</div>
						<div class="Box-sc-5vx4ls-0 RootNavigationBar__RootNavItemWrapper-sc-1tris5i-0 cGOgLs bOsaqT">
							<div display="flex"
								class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 dPVYbu fCPAWO Link__StyledLink-sc-38tiy-0 kWnpZi">
								<a target="_self"
									href="/docs/partners"><span display="flex" width="72" height="72" class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 dLhSPJ enkULn"><svg width="16" height="16" viewBox="0 0 16 12" fill="none" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" clip-rule="evenodd" d="M6.14316 2.96699C6.14316 3.56757 5.6563 4.05443 5.05572 4.05443C4.45515 4.05443 3.96828 3.56757 3.96828 2.96699C3.96828 2.36642 4.45515 1.87955 5.05572 1.87955C5.6563 1.87955 6.14316 2.36642 6.14316 2.96699ZM7.2306 2.96699C7.2306 4.16815 6.25687 5.14188 5.05572 5.14188C3.85457 5.14188 2.88084 4.16815 2.88084 2.96699C2.88084 1.76585 3.85457 0.792114 5.05572 0.792114C6.25687 0.792114 7.2306 1.76585 7.2306 2.96699ZM11.9831 2.96699C11.9831 3.56757 11.4963 4.05443 10.8956 4.05443C10.2951 4.05443 9.80817 3.56757 9.80817 2.96699C9.80817 2.36642 10.2951 1.87955 10.8956 1.87955C11.4963 1.87955 11.9831 2.36642 11.9831 2.96699ZM13.0706 2.96699C13.0706 4.16815 12.0968 5.14188 10.8956 5.14188C9.69448 5.14188 8.72077 4.16815 8.72077 2.96699C8.72077 1.76585 9.69448 0.792114 10.8956 0.792114C12.0968 0.792114 13.0706 1.76585 13.0706 2.96699ZM5.05572 7.55833C3.14277 7.55833 1.59203 9.10908 1.59203 11.0221C1.59203 11.4002 1.28548 11.7067 0.907341 11.7067C0.529199 11.7067 0.222656 11.4002 0.222656 11.0221C0.222656 8.35282 2.3865 6.18899 5.05572 6.18899C6.15283 6.18899 7.16454 6.55451 7.97573 7.17051C8.53686 6.74455 9.19466 6.43788 9.91101 6.28953C10.2295 6.22348 10.5589 6.18899 10.8956 6.18899C13.5649 6.18899 15.7287 8.35282 15.7287 11.0221C15.7287 11.4002 15.4222 11.7067 15.0441 11.7067C14.6659 11.7067 14.3594 11.4002 14.3594 11.0221C14.3594 9.10908 12.8086 7.55833 10.8956 7.55833C10.6528 7.55833 10.4164 7.58322 10.1888 7.63042C9.73732 7.72393 9.31759 7.90553 8.94843 8.15699C9.53946 8.95877 9.88879 9.94962 9.88879 11.0221C9.88879 11.4002 9.58221 11.7067 9.20408 11.7067C8.82596 11.7067 8.51942 11.4002 8.51942 11.0221C8.51942 9.10908 6.96867 7.55833 5.05572 7.55833Z" fill="#FFF" stroke-width="0.2"></path></svg><span class="Text-sc-1g8cvhx-0 cmLnxL">Partners</span></span></a>
							</div>
						</div>
						<div class="Box-sc-5vx4ls-0 RootNavigationBar__RootNavItemWrapper-sc-1tris5i-0 cGOgLs bOsaqT">
							<div display="flex"
								class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 dPVYbu fCPAWO Link__StyledLink-sc-38tiy-0 kWnpZi">
								<a target="_self"
									href="/docs/api"><span display="flex" width="72" height="72" class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 dLhSPJ enkULn"><svg width="16" height="16" viewBox="0 0 16 12" fill="none" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" clip-rule="evenodd" d="M10.3588 0.292599C10.6882 0.42683 10.8465 0.80267 10.7122 1.13207L6.45596 11.5766C6.32173 11.9061 5.94589 12.0643 5.6165 11.9301C5.2871 11.7958 5.12889 11.42 5.26312 11.0906L9.51934 0.645976C9.65357 0.316581 10.0295 0.158376 10.3588 0.292599ZM11.4876 3.11686C11.2721 3.39988 11.327 3.80397 11.61 4.01941L14.4822 6.20571L11.6174 8.32224C11.3313 8.53362 11.2707 8.93691 11.4821 9.22295C11.6934 9.50909 12.0967 9.56962 12.3828 9.35824L15.3377 7.17513C15.9833 6.69815 15.9903 5.73487 15.3515 5.24864L12.3902 2.99447C12.1072 2.77904 11.7031 2.83383 11.4876 3.11686ZM4.39013 3.57496C4.67316 3.35952 4.72795 2.95543 4.51251 2.67241C4.29707 2.38939 3.89299 2.3346 3.60996 2.55003L0.648612 4.80419C0.00985824 5.29042 0.0167586 6.25371 0.662413 6.73069L3.61734 8.9138C3.90342 9.12518 4.30669 9.06464 4.51805 8.77851C4.72941 8.49246 4.66883 8.08918 4.38275 7.8778L1.51791 5.76126L4.39013 3.57496Z" fill="#FFF"></path></svg><span class="Text-sc-1g8cvhx-0 cmLnxL">Developer Tools</span></span></a>
							</div>
						</div>
					</nav>
					<nav width="256" height="calc(100%)" overflow="auto" id="navTreeParent"
						class="Box-sc-5vx4ls-0 vOvvs">
						<nav class="Box-sc-5vx4ls-0 cGOgLs">
							<div
								class="Box-sc-5vx4ls-0 SidebarNavLink__SidebarnavLinkContainer-sc-pt5di4-0 bQnGvS fWgtQP">
								<div display="flex"
									class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 dPVYbu fCPAWO Link__StyledLink-sc-38tiy-0 kWnpZi">
									<a id="payments-sidebar" target="_self"
										href="/docs/payments"><span class="Text-sc-1g8cvhx-0 SidebarNavLink__SidebarnavLinkText-sc-pt5di4-1 bsHdmV kVxEKo">Razorpay Payments</span></a>
								</div>
							</div>
							<div class="Box-sc-5vx4ls-0 jiMkSI">
								<div data-state="closed">
									<div aria-controls="radix-id-2322785538-4610" aria-expanded="false"
										data-state="closed"
										class="Box-sc-5vx4ls-0 cGOgLs Trigger__CollapsibleTrigger-sc-zrl3ha-0 HBTNX">
										<div display="flex"
											class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 jnDyMP kqsqjK NavigationTree__StyledFlex-sc-1f9wbbd-1 bktzmf">
											<div class="Box-sc-5vx4ls-0 hZRMgn"><svg width="12" height="12"
													viewBox="0 0 10 8" fill="none" xmlns="http://www.w3.org/2000/svg"
													data-testid="double-chevron-right">
													<path
														d="M1.21936 0.195262C0.940416 -0.0650874 0.488155 -0.0650874 0.209209 0.195262C-0.0697365 0.455612 -0.0697365 0.877722 0.209209 1.13807L3.27556 4L0.209209 6.86193C-0.0697365 7.12228 -0.0697365 7.54439 0.209209 7.80474C0.488155 8.06509 0.940416 8.06509 1.21936 7.80474L4.79079 4.4714C5.06974 4.21106 5.06974 3.78894 4.79079 3.5286L1.21936 0.195262Z"
														fill="hsla(214, 18%, 69%, 1)"></path>
													<path
														d="M6.21936 0.195262C5.94042 -0.0650874 5.48816 -0.0650874 5.20921 0.195262C4.93026 0.455612 4.93026 0.877722 5.20921 1.13807L8.27556 4L5.20921 6.86193C4.93026 7.12228 4.93026 7.54439 5.20921 7.80474C5.48816 8.06509 5.94042 8.06509 6.21936 7.80474L9.79079 4.4714C10.0697 4.21106 10.0697 3.78894 9.79079 3.5286L6.21936 0.195262Z"
														fill="hsla(214, 18%, 69%, 1)"></path>
												</svg></div>
											<p
												class="Text-sc-1g8cvhx-0 NavigationTree__NavNodeCollapsibleTriggerText-sc-1f9wbbd-2 HSevc coZHyU">
												Sign Up</p>
										</div>
									</div>
									<div data-state="closed" id="radix-id-2322785538-4610" hidden=""
										class="Content__CollapsibleContent-sc-1bkq2us-0 eWXbsW"></div>
								</div>
							</div>
							<div class="Box-sc-5vx4ls-0 jiMkSI">
								<div data-state="closed">
									<div aria-controls="radix-id-2322785538-4611" aria-expanded="false"
										data-state="closed"
										class="Box-sc-5vx4ls-0 cGOgLs Trigger__CollapsibleTrigger-sc-zrl3ha-0 HBTNX">
										<div display="flex"
											class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 jnDyMP kqsqjK NavigationTree__StyledFlex-sc-1f9wbbd-1 bktzmf">
											<div class="Box-sc-5vx4ls-0 hZRMgn"><svg width="12" height="12"
													viewBox="0 0 10 8" fill="none" xmlns="http://www.w3.org/2000/svg"
													data-testid="double-chevron-right">
													<path
														d="M1.21936 0.195262C0.940416 -0.0650874 0.488155 -0.0650874 0.209209 0.195262C-0.0697365 0.455612 -0.0697365 0.877722 0.209209 1.13807L3.27556 4L0.209209 6.86193C-0.0697365 7.12228 -0.0697365 7.54439 0.209209 7.80474C0.488155 8.06509 0.940416 8.06509 1.21936 7.80474L4.79079 4.4714C5.06974 4.21106 5.06974 3.78894 4.79079 3.5286L1.21936 0.195262Z"
														fill="hsla(214, 18%, 69%, 1)"></path>
													<path
														d="M6.21936 0.195262C5.94042 -0.0650874 5.48816 -0.0650874 5.20921 0.195262C4.93026 0.455612 4.93026 0.877722 5.20921 1.13807L8.27556 4L5.20921 6.86193C4.93026 7.12228 4.93026 7.54439 5.20921 7.80474C5.48816 8.06509 5.94042 8.06509 6.21936 7.80474L9.79079 4.4714C10.0697 4.21106 10.0697 3.78894 9.79079 3.5286L6.21936 0.195262Z"
														fill="hsla(214, 18%, 69%, 1)"></path>
												</svg></div>
											<p
												class="Text-sc-1g8cvhx-0 NavigationTree__NavNodeCollapsibleTriggerText-sc-1f9wbbd-2 HSevc coZHyU">
												Dashboard</p>
										</div>
									</div>
									<div data-state="closed" id="radix-id-2322785538-4611" hidden=""
										class="Content__CollapsibleContent-sc-1bkq2us-0 eWXbsW"></div>
								</div>
							</div>
							<div class="Box-sc-5vx4ls-0 jiMkSI">
								<div data-state="closed">
									<div aria-controls="radix-id-2322785538-4612" aria-expanded="false"
										data-state="closed"
										class="Box-sc-5vx4ls-0 cGOgLs Trigger__CollapsibleTrigger-sc-zrl3ha-0 HBTNX">
										<div display="flex"
											class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 jnDyMP kqsqjK NavigationTree__StyledFlex-sc-1f9wbbd-1 bktzmf">
											<div class="Box-sc-5vx4ls-0 hZRMgn"><svg width="12" height="12"
													viewBox="0 0 10 8" fill="none" xmlns="http://www.w3.org/2000/svg"
													data-testid="double-chevron-right">
													<path
														d="M1.21936 0.195262C0.940416 -0.0650874 0.488155 -0.0650874 0.209209 0.195262C-0.0697365 0.455612 -0.0697365 0.877722 0.209209 1.13807L3.27556 4L0.209209 6.86193C-0.0697365 7.12228 -0.0697365 7.54439 0.209209 7.80474C0.488155 8.06509 0.940416 8.06509 1.21936 7.80474L4.79079 4.4714C5.06974 4.21106 5.06974 3.78894 4.79079 3.5286L1.21936 0.195262Z"
														fill="hsla(214, 18%, 69%, 1)"></path>
													<path
														d="M6.21936 0.195262C5.94042 -0.0650874 5.48816 -0.0650874 5.20921 0.195262C4.93026 0.455612 4.93026 0.877722 5.20921 1.13807L8.27556 4L5.20921 6.86193C4.93026 7.12228 4.93026 7.54439 5.20921 7.80474C5.48816 8.06509 5.94042 8.06509 6.21936 7.80474L9.79079 4.4714C10.0697 4.21106 10.0697 3.78894 9.79079 3.5286L6.21936 0.195262Z"
														fill="hsla(214, 18%, 69%, 1)"></path>
												</svg></div>
											<p
												class="Text-sc-1g8cvhx-0 NavigationTree__NavNodeCollapsibleTriggerText-sc-1f9wbbd-2 HSevc coZHyU">
												Customers</p>
										</div>
									</div>
									<div data-state="closed" id="radix-id-2322785538-4612" hidden=""
										class="Content__CollapsibleContent-sc-1bkq2us-0 eWXbsW"></div>
								</div>
							</div>
							<div class="Box-sc-5vx4ls-0 jiMkSI">
								<div data-state="closed">
									<div aria-controls="radix-id-2322785538-4613" aria-expanded="false"
										data-state="closed"
										class="Box-sc-5vx4ls-0 cGOgLs Trigger__CollapsibleTrigger-sc-zrl3ha-0 HBTNX">
										<div display="flex"
											class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 jnDyMP kqsqjK NavigationTree__StyledFlex-sc-1f9wbbd-1 bktzmf">
											<div class="Box-sc-5vx4ls-0 hZRMgn"><svg width="12" height="12"
													viewBox="0 0 10 8" fill="none" xmlns="http://www.w3.org/2000/svg"
													data-testid="double-chevron-right">
													<path
														d="M1.21936 0.195262C0.940416 -0.0650874 0.488155 -0.0650874 0.209209 0.195262C-0.0697365 0.455612 -0.0697365 0.877722 0.209209 1.13807L3.27556 4L0.209209 6.86193C-0.0697365 7.12228 -0.0697365 7.54439 0.209209 7.80474C0.488155 8.06509 0.940416 8.06509 1.21936 7.80474L4.79079 4.4714C5.06974 4.21106 5.06974 3.78894 4.79079 3.5286L1.21936 0.195262Z"
														fill="hsla(214, 18%, 69%, 1)"></path>
													<path
														d="M6.21936 0.195262C5.94042 -0.0650874 5.48816 -0.0650874 5.20921 0.195262C4.93026 0.455612 4.93026 0.877722 5.20921 1.13807L8.27556 4L5.20921 6.86193C4.93026 7.12228 4.93026 7.54439 5.20921 7.80474C5.48816 8.06509 5.94042 8.06509 6.21936 7.80474L9.79079 4.4714C10.0697 4.21106 10.0697 3.78894 9.79079 3.5286L6.21936 0.195262Z"
														fill="hsla(214, 18%, 69%, 1)"></path>
												</svg></div>
											<p
												class="Text-sc-1g8cvhx-0 NavigationTree__NavNodeCollapsibleTriggerText-sc-1f9wbbd-2 HSevc coZHyU">
												Orders</p>
										</div>
									</div>
									<div data-state="closed" id="radix-id-2322785538-4613" hidden=""
										class="Content__CollapsibleContent-sc-1bkq2us-0 eWXbsW"></div>
								</div>
							</div>
							<div class="Box-sc-5vx4ls-0 jiMkSI">
								<div data-state="closed">
									<div aria-controls="radix-id-2322785538-4614" aria-expanded="false"
										data-state="closed"
										class="Box-sc-5vx4ls-0 cGOgLs Trigger__CollapsibleTrigger-sc-zrl3ha-0 HBTNX">
										<div display="flex"
											class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 jnDyMP kqsqjK NavigationTree__StyledFlex-sc-1f9wbbd-1 bktzmf">
											<div class="Box-sc-5vx4ls-0 hZRMgn"><svg width="12" height="12"
													viewBox="0 0 10 8" fill="none" xmlns="http://www.w3.org/2000/svg"
													data-testid="double-chevron-right">
													<path
														d="M1.21936 0.195262C0.940416 -0.0650874 0.488155 -0.0650874 0.209209 0.195262C-0.0697365 0.455612 -0.0697365 0.877722 0.209209 1.13807L3.27556 4L0.209209 6.86193C-0.0697365 7.12228 -0.0697365 7.54439 0.209209 7.80474C0.488155 8.06509 0.940416 8.06509 1.21936 7.80474L4.79079 4.4714C5.06974 4.21106 5.06974 3.78894 4.79079 3.5286L1.21936 0.195262Z"
														fill="hsla(214, 18%, 69%, 1)"></path>
													<path
														d="M6.21936 0.195262C5.94042 -0.0650874 5.48816 -0.0650874 5.20921 0.195262C4.93026 0.455612 4.93026 0.877722 5.20921 1.13807L8.27556 4L5.20921 6.86193C4.93026 7.12228 4.93026 7.54439 5.20921 7.80474C5.48816 8.06509 5.94042 8.06509 6.21936 7.80474L9.79079 4.4714C10.0697 4.21106 10.0697 3.78894 9.79079 3.5286L6.21936 0.195262Z"
														fill="hsla(214, 18%, 69%, 1)"></path>
												</svg></div>
											<p
												class="Text-sc-1g8cvhx-0 NavigationTree__NavNodeCollapsibleTriggerText-sc-1f9wbbd-2 HSevc coZHyU">
												Payments</p>
										</div>
									</div>
									<div data-state="closed" id="radix-id-2322785538-4614" hidden=""
										class="Content__CollapsibleContent-sc-1bkq2us-0 eWXbsW"></div>
								</div>
							</div>
							<div class="Box-sc-5vx4ls-0 jiMkSI">
								<div data-state="closed">
									<div aria-controls="radix-id-2322785538-4615" aria-expanded="false"
										data-state="closed"
										class="Box-sc-5vx4ls-0 cGOgLs Trigger__CollapsibleTrigger-sc-zrl3ha-0 HBTNX">
										<div display="flex"
											class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 jnDyMP kqsqjK NavigationTree__StyledFlex-sc-1f9wbbd-1 bktzmf">
											<div class="Box-sc-5vx4ls-0 hZRMgn"><svg width="12" height="12"
													viewBox="0 0 10 8" fill="none" xmlns="http://www.w3.org/2000/svg"
													data-testid="double-chevron-right">
													<path
														d="M1.21936 0.195262C0.940416 -0.0650874 0.488155 -0.0650874 0.209209 0.195262C-0.0697365 0.455612 -0.0697365 0.877722 0.209209 1.13807L3.27556 4L0.209209 6.86193C-0.0697365 7.12228 -0.0697365 7.54439 0.209209 7.80474C0.488155 8.06509 0.940416 8.06509 1.21936 7.80474L4.79079 4.4714C5.06974 4.21106 5.06974 3.78894 4.79079 3.5286L1.21936 0.195262Z"
														fill="hsla(214, 18%, 69%, 1)"></path>
													<path
														d="M6.21936 0.195262C5.94042 -0.0650874 5.48816 -0.0650874 5.20921 0.195262C4.93026 0.455612 4.93026 0.877722 5.20921 1.13807L8.27556 4L5.20921 6.86193C4.93026 7.12228 4.93026 7.54439 5.20921 7.80474C5.48816 8.06509 5.94042 8.06509 6.21936 7.80474L9.79079 4.4714C10.0697 4.21106 10.0697 3.78894 9.79079 3.5286L6.21936 0.195262Z"
														fill="hsla(214, 18%, 69%, 1)"></path>
												</svg></div>
											<p
												class="Text-sc-1g8cvhx-0 NavigationTree__NavNodeCollapsibleTriggerText-sc-1f9wbbd-2 HSevc coZHyU">
												Payment Methods</p>
										</div>
									</div>
									<div data-state="closed" id="radix-id-2322785538-4615" hidden=""
										class="Content__CollapsibleContent-sc-1bkq2us-0 eWXbsW"></div>
								</div>
							</div>
							<div class="Box-sc-5vx4ls-0 jiMkSI">
								<div data-state="closed">
									<div aria-controls="radix-id-2322785538-4616" aria-expanded="false"
										data-state="closed"
										class="Box-sc-5vx4ls-0 cGOgLs Trigger__CollapsibleTrigger-sc-zrl3ha-0 HBTNX">
										<div display="flex"
											class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 jnDyMP kqsqjK NavigationTree__StyledFlex-sc-1f9wbbd-1 bktzmf">
											<div class="Box-sc-5vx4ls-0 hZRMgn"><svg width="12" height="12"
													viewBox="0 0 10 8" fill="none" xmlns="http://www.w3.org/2000/svg"
													data-testid="double-chevron-right">
													<path
														d="M1.21936 0.195262C0.940416 -0.0650874 0.488155 -0.0650874 0.209209 0.195262C-0.0697365 0.455612 -0.0697365 0.877722 0.209209 1.13807L3.27556 4L0.209209 6.86193C-0.0697365 7.12228 -0.0697365 7.54439 0.209209 7.80474C0.488155 8.06509 0.940416 8.06509 1.21936 7.80474L4.79079 4.4714C5.06974 4.21106 5.06974 3.78894 4.79079 3.5286L1.21936 0.195262Z"
														fill="hsla(214, 18%, 69%, 1)"></path>
													<path
														d="M6.21936 0.195262C5.94042 -0.0650874 5.48816 -0.0650874 5.20921 0.195262C4.93026 0.455612 4.93026 0.877722 5.20921 1.13807L8.27556 4L5.20921 6.86193C4.93026 7.12228 4.93026 7.54439 5.20921 7.80474C5.48816 8.06509 5.94042 8.06509 6.21936 7.80474L9.79079 4.4714C10.0697 4.21106 10.0697 3.78894 9.79079 3.5286L6.21936 0.195262Z"
														fill="hsla(214, 18%, 69%, 1)"></path>
												</svg></div>
											<p
												class="Text-sc-1g8cvhx-0 NavigationTree__NavNodeCollapsibleTriggerText-sc-1f9wbbd-2 HSevc coZHyU">
												Settlements</p>
										</div>
									</div>
									<div data-state="closed" id="radix-id-2322785538-4616" hidden=""
										class="Content__CollapsibleContent-sc-1bkq2us-0 eWXbsW"></div>
								</div>
							</div>
							<div class="Box-sc-5vx4ls-0 jiMkSI">
								<div data-state="closed">
									<div aria-controls="radix-id-2322785538-4617" aria-expanded="false"
										data-state="closed"
										class="Box-sc-5vx4ls-0 cGOgLs Trigger__CollapsibleTrigger-sc-zrl3ha-0 HBTNX">
										<div display="flex"
											class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 jnDyMP kqsqjK NavigationTree__StyledFlex-sc-1f9wbbd-1 bktzmf">
											<div class="Box-sc-5vx4ls-0 hZRMgn"><svg width="12" height="12"
													viewBox="0 0 10 8" fill="none" xmlns="http://www.w3.org/2000/svg"
													data-testid="double-chevron-right">
													<path
														d="M1.21936 0.195262C0.940416 -0.0650874 0.488155 -0.0650874 0.209209 0.195262C-0.0697365 0.455612 -0.0697365 0.877722 0.209209 1.13807L3.27556 4L0.209209 6.86193C-0.0697365 7.12228 -0.0697365 7.54439 0.209209 7.80474C0.488155 8.06509 0.940416 8.06509 1.21936 7.80474L4.79079 4.4714C5.06974 4.21106 5.06974 3.78894 4.79079 3.5286L1.21936 0.195262Z"
														fill="hsla(214, 18%, 69%, 1)"></path>
													<path
														d="M6.21936 0.195262C5.94042 -0.0650874 5.48816 -0.0650874 5.20921 0.195262C4.93026 0.455612 4.93026 0.877722 5.20921 1.13807L8.27556 4L5.20921 6.86193C4.93026 7.12228 4.93026 7.54439 5.20921 7.80474C5.48816 8.06509 5.94042 8.06509 6.21936 7.80474L9.79079 4.4714C10.0697 4.21106 10.0697 3.78894 9.79079 3.5286L6.21936 0.195262Z"
														fill="hsla(214, 18%, 69%, 1)"></path>
												</svg></div>
											<p
												class="Text-sc-1g8cvhx-0 NavigationTree__NavNodeCollapsibleTriggerText-sc-1f9wbbd-2 HSevc coZHyU">
												Refunds</p>
										</div>
									</div>
									<div data-state="closed" id="radix-id-2322785538-4617" hidden=""
										class="Content__CollapsibleContent-sc-1bkq2us-0 eWXbsW"></div>
								</div>
							</div>
							<div class="Box-sc-5vx4ls-0 jiMkSI">
								<div data-state="closed">
									<div aria-controls="radix-id-2322785538-4618" aria-expanded="false"
										data-state="closed"
										class="Box-sc-5vx4ls-0 cGOgLs Trigger__CollapsibleTrigger-sc-zrl3ha-0 HBTNX">
										<div display="flex"
											class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 jnDyMP kqsqjK NavigationTree__StyledFlex-sc-1f9wbbd-1 bktzmf">
											<div class="Box-sc-5vx4ls-0 hZRMgn"><svg width="12" height="12"
													viewBox="0 0 10 8" fill="none" xmlns="http://www.w3.org/2000/svg"
													data-testid="double-chevron-right">
													<path
														d="M1.21936 0.195262C0.940416 -0.0650874 0.488155 -0.0650874 0.209209 0.195262C-0.0697365 0.455612 -0.0697365 0.877722 0.209209 1.13807L3.27556 4L0.209209 6.86193C-0.0697365 7.12228 -0.0697365 7.54439 0.209209 7.80474C0.488155 8.06509 0.940416 8.06509 1.21936 7.80474L4.79079 4.4714C5.06974 4.21106 5.06974 3.78894 4.79079 3.5286L1.21936 0.195262Z"
														fill="hsla(214, 18%, 69%, 1)"></path>
													<path
														d="M6.21936 0.195262C5.94042 -0.0650874 5.48816 -0.0650874 5.20921 0.195262C4.93026 0.455612 4.93026 0.877722 5.20921 1.13807L8.27556 4L5.20921 6.86193C4.93026 7.12228 4.93026 7.54439 5.20921 7.80474C5.48816 8.06509 5.94042 8.06509 6.21936 7.80474L9.79079 4.4714C10.0697 4.21106 10.0697 3.78894 9.79079 3.5286L6.21936 0.195262Z"
														fill="hsla(214, 18%, 69%, 1)"></path>
												</svg></div>
											<p
												class="Text-sc-1g8cvhx-0 NavigationTree__NavNodeCollapsibleTriggerText-sc-1f9wbbd-2 HSevc coZHyU">
												Disputes</p>
										</div>
									</div>
									<div data-state="closed" id="radix-id-2322785538-4618" hidden=""
										class="Content__CollapsibleContent-sc-1bkq2us-0 eWXbsW"></div>
								</div>
							</div>
							<div class="Box-sc-5vx4ls-0 jiMkSI">
								<div data-state="closed">
									<div aria-controls="radix-id-2322785538-4619" aria-expanded="false"
										data-state="closed"
										class="Box-sc-5vx4ls-0 cGOgLs Trigger__CollapsibleTrigger-sc-zrl3ha-0 HBTNX">
										<div display="flex"
											class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 jnDyMP kqsqjK NavigationTree__StyledFlex-sc-1f9wbbd-1 bktzmf">
											<div class="Box-sc-5vx4ls-0 hZRMgn"><svg width="12" height="12"
													viewBox="0 0 10 8" fill="none" xmlns="http://www.w3.org/2000/svg"
													data-testid="double-chevron-right">
													<path
														d="M1.21936 0.195262C0.940416 -0.0650874 0.488155 -0.0650874 0.209209 0.195262C-0.0697365 0.455612 -0.0697365 0.877722 0.209209 1.13807L3.27556 4L0.209209 6.86193C-0.0697365 7.12228 -0.0697365 7.54439 0.209209 7.80474C0.488155 8.06509 0.940416 8.06509 1.21936 7.80474L4.79079 4.4714C5.06974 4.21106 5.06974 3.78894 4.79079 3.5286L1.21936 0.195262Z"
														fill="hsla(214, 18%, 69%, 1)"></path>
													<path
														d="M6.21936 0.195262C5.94042 -0.0650874 5.48816 -0.0650874 5.20921 0.195262C4.93026 0.455612 4.93026 0.877722 5.20921 1.13807L8.27556 4L5.20921 6.86193C4.93026 7.12228 4.93026 7.54439 5.20921 7.80474C5.48816 8.06509 5.94042 8.06509 6.21936 7.80474L9.79079 4.4714C10.0697 4.21106 10.0697 3.78894 9.79079 3.5286L6.21936 0.195262Z"
														fill="hsla(214, 18%, 69%, 1)"></path>
												</svg></div>
											<p
												class="Text-sc-1g8cvhx-0 NavigationTree__NavNodeCollapsibleTriggerText-sc-1f9wbbd-2 HSevc coZHyU">
												Payment Gateway</p>
										</div>
									</div>
									<div data-state="closed" id="radix-id-2322785538-4619" hidden=""
										class="Content__CollapsibleContent-sc-1bkq2us-0 eWXbsW"></div>
								</div>
							</div>
							<div class="Box-sc-5vx4ls-0 jiMkSI">
								<div data-state="open">
									<div aria-controls="radix-id-2322785538-4620" aria-expanded="true" data-state="open"
										class="Box-sc-5vx4ls-0 cGOgLs Trigger__CollapsibleTrigger-sc-zrl3ha-0 HBTNX">
										<div display="flex"
											class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 jnDyMP kqsqjK NavigationTree__StyledFlex-sc-1f9wbbd-1 iZcbJV">
											<div class="Box-sc-5vx4ls-0 hZRMgn"><svg width="12" height="12"
													viewBox="0 0 8 10" fill="none" xmlns="http://www.w3.org/2000/svg"
													data-testid="double-chevron-down">
													<path
														d="M7.80474 1.21936C8.06509 0.940416 8.06509 0.488155 7.80474 0.209209C7.54439 -0.0697365 7.12228 -0.0697365 6.86193 0.209209L4 3.27556L1.13807 0.209209C0.877722 -0.0697368 0.455611 -0.0697368 0.195262 0.209209C-0.0650879 0.488155 -0.0650879 0.940416 0.195262 1.21936L3.5286 4.79079C3.78894 5.06974 4.21105 5.06974 4.4714 4.79079L7.80474 1.21936Z"
														fill="hsla(217, 18%, 45%, 1)"></path>
													<path
														d="M7.80474 6.21936C8.06509 5.94042 8.06509 5.48816 7.80474 5.20921C7.54439 4.93026 7.12228 4.93026 6.86193 5.20921L4 8.27556L1.13807 5.20921C0.877721 4.93026 0.455611 4.93026 0.195262 5.20921C-0.0650881 5.48816 -0.0650881 5.94042 0.195262 6.21936L3.5286 9.79079C3.78894 10.0697 4.21105 10.0697 4.4714 9.79079L7.80474 6.21936Z"
														fill="hsla(217, 18%, 45%, 1)"></path>
												</svg></div>
											<p
												class="Text-sc-1g8cvhx-0 NavigationTree__NavNodeCollapsibleTriggerText-sc-1f9wbbd-2 ieCmBj hGeEcs">
												Ecommerce Plugins</p>
										</div>
									</div>
									<div data-state="open" id="radix-id-2322785538-4620"
										class="Content__CollapsibleContent-sc-1bkq2us-0 eWXbsW">
										<div class="Box-sc-5vx4ls-0 iFgnvD">
											<div display="flex"
												class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 dPVYbu gyXFoV NavigationTree__NavNodesContainer-sc-1f9wbbd-0 jVrtuA">
												<nav class="Box-sc-5vx4ls-0 cGOgLs">
													<div
														class="Box-sc-5vx4ls-0 SidebarNavLink__SidebarnavLinkContainer-sc-pt5di4-0 bQnGvS fWgtQP">
														<div display="flex"
															class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 dPVYbu fCPAWO Link__StyledLink-sc-38tiy-0 kWnpZi">
															<a id="payments/payment-gateway/ecommerce-plugins-sidebar"
																target="_self"
																href="/docs/payments/payment-gateway/ecommerce-plugins"><span class="Text-sc-1g8cvhx-0 SidebarNavLink__SidebarnavLinkText-sc-pt5di4-1 cnaGRq kkEfVJ">About Ecommerce Plugins</span></a>
														</div>
													</div>
													<div class="Box-sc-5vx4ls-0 jiMkSI">
														<div data-state="closed">
															<div aria-controls="radix-id-2322785538-4621"
																aria-expanded="false" data-state="closed"
																class="Box-sc-5vx4ls-0 cGOgLs Trigger__CollapsibleTrigger-sc-zrl3ha-0 HBTNX">
																<div display="flex"
																	class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 jnDyMP kqsqjK NavigationTree__StyledFlex-sc-1f9wbbd-1 bktzmf">
																	<div class="Box-sc-5vx4ls-0 hZRMgn"><svg width="12"
																			height="12" viewBox="0 0 24 24" fill="none"
																			xmlns="http://www.w3.org/2000/svg">
																			<path fill-rule="evenodd"
																				clip-rule="evenodd"
																				d="M8.293 5.293a1 1 0 0 1 1.414 0l6 6a1 1 0 0 1 0 1.414l-6 6a1 1 0 0 1-1.414-1.414L13.586 12 8.293 6.707a1 1 0 0 1 0-1.414Z"
																				fill="hsla(214, 18%, 69%, 1)"></path>
																		</svg></div>
																	<p
																		class="Text-sc-1g8cvhx-0 NavigationTree__NavNodeCollapsibleTriggerText-sc-1f9wbbd-2 HSevc gknCtx">
																		Arastta</p>
																</div>
															</div>
															<div data-state="closed" id="radix-id-2322785538-4621"
																hidden=""
																class="Content__CollapsibleContent-sc-1bkq2us-0 eWXbsW">
															</div>
														</div>
													</div>
													<div class="Box-sc-5vx4ls-0 jiMkSI">
														<div data-state="closed">
															<div aria-controls="radix-id-2322785538-4622"
																aria-expanded="false" data-state="closed"
																class="Box-sc-5vx4ls-0 cGOgLs Trigger__CollapsibleTrigger-sc-zrl3ha-0 HBTNX">
																<div display="flex"
																	class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 jnDyMP kqsqjK NavigationTree__StyledFlex-sc-1f9wbbd-1 bktzmf">
																	<div class="Box-sc-5vx4ls-0 hZRMgn"><svg width="12"
																			height="12" viewBox="0 0 24 24" fill="none"
																			xmlns="http://www.w3.org/2000/svg">
																			<path fill-rule="evenodd"
																				clip-rule="evenodd"
																				d="M8.293 5.293a1 1 0 0 1 1.414 0l6 6a1 1 0 0 1 0 1.414l-6 6a1 1 0 0 1-1.414-1.414L13.586 12 8.293 6.707a1 1 0 0 1 0-1.414Z"
																				fill="hsla(214, 18%, 69%, 1)"></path>
																		</svg></div>
																	<p
																		class="Text-sc-1g8cvhx-0 NavigationTree__NavNodeCollapsibleTriggerText-sc-1f9wbbd-2 HSevc gknCtx">
																		Build Your Own</p>
																</div>
															</div>
															<div data-state="closed" id="radix-id-2322785538-4622"
																hidden=""
																class="Content__CollapsibleContent-sc-1bkq2us-0 eWXbsW">
															</div>
														</div>
													</div>
													<div class="Box-sc-5vx4ls-0 jiMkSI">
														<div data-state="closed">
															<div aria-controls="radix-id-2322785538-4623"
																aria-expanded="false" data-state="closed"
																class="Box-sc-5vx4ls-0 cGOgLs Trigger__CollapsibleTrigger-sc-zrl3ha-0 HBTNX">
																<div display="flex"
																	class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 jnDyMP kqsqjK NavigationTree__StyledFlex-sc-1f9wbbd-1 bktzmf">
																	<div class="Box-sc-5vx4ls-0 hZRMgn"><svg width="12"
																			height="12" viewBox="0 0 24 24" fill="none"
																			xmlns="http://www.w3.org/2000/svg">
																			<path fill-rule="evenodd"
																				clip-rule="evenodd"
																				d="M8.293 5.293a1 1 0 0 1 1.414 0l6 6a1 1 0 0 1 0 1.414l-6 6a1 1 0 0 1-1.414-1.414L13.586 12 8.293 6.707a1 1 0 0 1 0-1.414Z"
																				fill="hsla(214, 18%, 69%, 1)"></path>
																		</svg></div>
																	<p
																		class="Text-sc-1g8cvhx-0 NavigationTree__NavNodeCollapsibleTriggerText-sc-1f9wbbd-2 HSevc gknCtx">
																		BigCommerce</p>
																</div>
															</div>
															<div data-state="closed" id="radix-id-2322785538-4623"
																hidden=""
																class="Content__CollapsibleContent-sc-1bkq2us-0 eWXbsW">
															</div>
														</div>
													</div>
													<div class="Box-sc-5vx4ls-0 jiMkSI">
														<div data-state="closed">
															<div aria-controls="radix-id-2322785538-4624"
																aria-expanded="false" data-state="closed"
																class="Box-sc-5vx4ls-0 cGOgLs Trigger__CollapsibleTrigger-sc-zrl3ha-0 HBTNX">
																<div display="flex"
																	class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 jnDyMP kqsqjK NavigationTree__StyledFlex-sc-1f9wbbd-1 bktzmf">
																	<div class="Box-sc-5vx4ls-0 hZRMgn"><svg width="12"
																			height="12" viewBox="0 0 24 24" fill="none"
																			xmlns="http://www.w3.org/2000/svg">
																			<path fill-rule="evenodd"
																				clip-rule="evenodd"
																				d="M8.293 5.293a1 1 0 0 1 1.414 0l6 6a1 1 0 0 1 0 1.414l-6 6a1 1 0 0 1-1.414-1.414L13.586 12 8.293 6.707a1 1 0 0 1 0-1.414Z"
																				fill="hsla(214, 18%, 69%, 1)"></path>
																		</svg></div>
																	<p
																		class="Text-sc-1g8cvhx-0 NavigationTree__NavNodeCollapsibleTriggerText-sc-1f9wbbd-2 HSevc gknCtx">
																		Drupal Commerce</p>
																</div>
															</div>
															<div data-state="closed" id="radix-id-2322785538-4624"
																hidden=""
																class="Content__CollapsibleContent-sc-1bkq2us-0 eWXbsW">
															</div>
														</div>
													</div>
													<div class="Box-sc-5vx4ls-0 jiMkSI">
														<div data-state="closed">
															<div aria-controls="radix-id-2322785538-4625"
																aria-expanded="false" data-state="closed"
																class="Box-sc-5vx4ls-0 cGOgLs Trigger__CollapsibleTrigger-sc-zrl3ha-0 HBTNX">
																<div display="flex"
																	class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 jnDyMP kqsqjK NavigationTree__StyledFlex-sc-1f9wbbd-1 bktzmf">
																	<div class="Box-sc-5vx4ls-0 hZRMgn"><svg width="12"
																			height="12" viewBox="0 0 24 24" fill="none"
																			xmlns="http://www.w3.org/2000/svg">
																			<path fill-rule="evenodd"
																				clip-rule="evenodd"
																				d="M8.293 5.293a1 1 0 0 1 1.414 0l6 6a1 1 0 0 1 0 1.414l-6 6a1 1 0 0 1-1.414-1.414L13.586 12 8.293 6.707a1 1 0 0 1 0-1.414Z"
																				fill="hsla(214, 18%, 69%, 1)"></path>
																		</svg></div>
																	<p
																		class="Text-sc-1g8cvhx-0 NavigationTree__NavNodeCollapsibleTriggerText-sc-1f9wbbd-2 HSevc gknCtx">
																		Easy Digital Downloads</p>
																</div>
															</div>
															<div data-state="closed" id="radix-id-2322785538-4625"
																hidden=""
																class="Content__CollapsibleContent-sc-1bkq2us-0 eWXbsW">
															</div>
														</div>
													</div>
													<div class="Box-sc-5vx4ls-0 jiMkSI">
														<div data-state="closed">
															<div aria-controls="radix-id-2322785538-4626"
																aria-expanded="false" data-state="closed"
																class="Box-sc-5vx4ls-0 cGOgLs Trigger__CollapsibleTrigger-sc-zrl3ha-0 HBTNX">
																<div display="flex"
																	class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 jnDyMP kqsqjK NavigationTree__StyledFlex-sc-1f9wbbd-1 bktzmf">
																	<div class="Box-sc-5vx4ls-0 hZRMgn"><svg width="12"
																			height="12" viewBox="0 0 24 24" fill="none"
																			xmlns="http://www.w3.org/2000/svg">
																			<path fill-rule="evenodd"
																				clip-rule="evenodd"
																				d="M8.293 5.293a1 1 0 0 1 1.414 0l6 6a1 1 0 0 1 0 1.414l-6 6a1 1 0 0 1-1.414-1.414L13.586 12 8.293 6.707a1 1 0 0 1 0-1.414Z"
																				fill="hsla(214, 18%, 69%, 1)"></path>
																		</svg></div>
																	<p
																		class="Text-sc-1g8cvhx-0 NavigationTree__NavNodeCollapsibleTriggerText-sc-1f9wbbd-2 HSevc gknCtx">
																		CS-Cart</p>
																</div>
															</div>
															<div data-state="closed" id="radix-id-2322785538-4626"
																hidden=""
																class="Content__CollapsibleContent-sc-1bkq2us-0 eWXbsW">
															</div>
														</div>
													</div>
													<div class="Box-sc-5vx4ls-0 jiMkSI">
														<div data-state="closed">
															<div aria-controls="radix-id-2322785538-4627"
																aria-expanded="false" data-state="closed"
																class="Box-sc-5vx4ls-0 cGOgLs Trigger__CollapsibleTrigger-sc-zrl3ha-0 HBTNX">
																<div display="flex"
																	class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 jnDyMP kqsqjK NavigationTree__StyledFlex-sc-1f9wbbd-1 bktzmf">
																	<div class="Box-sc-5vx4ls-0 hZRMgn"><svg width="12"
																			height="12" viewBox="0 0 24 24" fill="none"
																			xmlns="http://www.w3.org/2000/svg">
																			<path fill-rule="evenodd"
																				clip-rule="evenodd"
																				d="M8.293 5.293a1 1 0 0 1 1.414 0l6 6a1 1 0 0 1 0 1.414l-6 6a1 1 0 0 1-1.414-1.414L13.586 12 8.293 6.707a1 1 0 0 1 0-1.414Z"
																				fill="hsla(214, 18%, 69%, 1)"></path>
																		</svg></div>
																	<p
																		class="Text-sc-1g8cvhx-0 NavigationTree__NavNodeCollapsibleTriggerText-sc-1f9wbbd-2 HSevc gknCtx">
																		Gravity Forms</p>
																</div>
															</div>
															<div data-state="closed" id="radix-id-2322785538-4627"
																hidden=""
																class="Content__CollapsibleContent-sc-1bkq2us-0 eWXbsW">
															</div>
														</div>
													</div>
													<div class="Box-sc-5vx4ls-0 jiMkSI">
														<div data-state="closed">
															<div aria-controls="radix-id-2322785538-4628"
																aria-expanded="false" data-state="closed"
																class="Box-sc-5vx4ls-0 cGOgLs Trigger__CollapsibleTrigger-sc-zrl3ha-0 HBTNX">
																<div display="flex"
																	class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 jnDyMP kqsqjK NavigationTree__StyledFlex-sc-1f9wbbd-1 bktzmf">
																	<div class="Box-sc-5vx4ls-0 hZRMgn"><svg width="12"
																			height="12" viewBox="0 0 24 24" fill="none"
																			xmlns="http://www.w3.org/2000/svg">
																			<path fill-rule="evenodd"
																				clip-rule="evenodd"
																				d="M8.293 5.293a1 1 0 0 1 1.414 0l6 6a1 1 0 0 1 0 1.414l-6 6a1 1 0 0 1-1.414-1.414L13.586 12 8.293 6.707a1 1 0 0 1 0-1.414Z"
																				fill="hsla(214, 18%, 69%, 1)"></path>
																		</svg></div>
																	<p
																		class="Text-sc-1g8cvhx-0 NavigationTree__NavNodeCollapsibleTriggerText-sc-1f9wbbd-2 HSevc gknCtx">
																		Magento</p>
																</div>
															</div>
															<div data-state="closed" id="radix-id-2322785538-4628"
																hidden=""
																class="Content__CollapsibleContent-sc-1bkq2us-0 eWXbsW">
															</div>
														</div>
													</div>
													<div class="Box-sc-5vx4ls-0 jiMkSI">
														<div data-state="closed">
															<div aria-controls="radix-id-2322785538-4629"
																aria-expanded="false" data-state="closed"
																class="Box-sc-5vx4ls-0 cGOgLs Trigger__CollapsibleTrigger-sc-zrl3ha-0 HBTNX">
																<div display="flex"
																	class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 jnDyMP kqsqjK NavigationTree__StyledFlex-sc-1f9wbbd-1 bktzmf">
																	<div class="Box-sc-5vx4ls-0 hZRMgn"><svg width="12"
																			height="12" viewBox="0 0 24 24" fill="none"
																			xmlns="http://www.w3.org/2000/svg">
																			<path fill-rule="evenodd"
																				clip-rule="evenodd"
																				d="M8.293 5.293a1 1 0 0 1 1.414 0l6 6a1 1 0 0 1 0 1.414l-6 6a1 1 0 0 1-1.414-1.414L13.586 12 8.293 6.707a1 1 0 0 1 0-1.414Z"
																				fill="hsla(214, 18%, 69%, 1)"></path>
																		</svg></div>
																	<p
																		class="Text-sc-1g8cvhx-0 NavigationTree__NavNodeCollapsibleTriggerText-sc-1f9wbbd-2 HSevc gknCtx">
																		OpenCart</p>
																</div>
															</div>
															<div data-state="closed" id="radix-id-2322785538-4629"
																hidden=""
																class="Content__CollapsibleContent-sc-1bkq2us-0 eWXbsW">
															</div>
														</div>
													</div>
													<div class="Box-sc-5vx4ls-0 jiMkSI">
														<div data-state="closed">
															<div aria-controls="radix-id-2322785538-4630"
																aria-expanded="false" data-state="closed"
																class="Box-sc-5vx4ls-0 cGOgLs Trigger__CollapsibleTrigger-sc-zrl3ha-0 HBTNX">
																<div display="flex"
																	class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 jnDyMP kqsqjK NavigationTree__StyledFlex-sc-1f9wbbd-1 bktzmf">
																	<div class="Box-sc-5vx4ls-0 hZRMgn"><svg width="12"
																			height="12" viewBox="0 0 24 24" fill="none"
																			xmlns="http://www.w3.org/2000/svg">
																			<path fill-rule="evenodd"
																				clip-rule="evenodd"
																				d="M8.293 5.293a1 1 0 0 1 1.414 0l6 6a1 1 0 0 1 0 1.414l-6 6a1 1 0 0 1-1.414-1.414L13.586 12 8.293 6.707a1 1 0 0 1 0-1.414Z"
																				fill="hsla(214, 18%, 69%, 1)"></path>
																		</svg></div>
																	<p
																		class="Text-sc-1g8cvhx-0 NavigationTree__NavNodeCollapsibleTriggerText-sc-1f9wbbd-2 HSevc gknCtx">
																		Prestashop</p>
																</div>
															</div>
															<div data-state="closed" id="radix-id-2322785538-4630"
																hidden=""
																class="Content__CollapsibleContent-sc-1bkq2us-0 eWXbsW">
															</div>
														</div>
													</div>
													<div class="Box-sc-5vx4ls-0 jiMkSI">
														<div data-state="closed">
															<div aria-controls="radix-id-2322785538-4631"
																aria-expanded="false" data-state="closed"
																class="Box-sc-5vx4ls-0 cGOgLs Trigger__CollapsibleTrigger-sc-zrl3ha-0 HBTNX">
																<div display="flex"
																	class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 jnDyMP kqsqjK NavigationTree__StyledFlex-sc-1f9wbbd-1 bktzmf">
																	<div class="Box-sc-5vx4ls-0 hZRMgn"><svg width="12"
																			height="12" viewBox="0 0 24 24" fill="none"
																			xmlns="http://www.w3.org/2000/svg">
																			<path fill-rule="evenodd"
																				clip-rule="evenodd"
																				d="M8.293 5.293a1 1 0 0 1 1.414 0l6 6a1 1 0 0 1 0 1.414l-6 6a1 1 0 0 1-1.414-1.414L13.586 12 8.293 6.707a1 1 0 0 1 0-1.414Z"
																				fill="hsla(214, 18%, 69%, 1)"></path>
																		</svg></div>
																	<p
																		class="Text-sc-1g8cvhx-0 NavigationTree__NavNodeCollapsibleTriggerText-sc-1f9wbbd-2 HSevc gknCtx">
																		Shopify - Razorpay Secure</p>
																</div>
															</div>
															<div data-state="closed" id="radix-id-2322785538-4631"
																hidden=""
																class="Content__CollapsibleContent-sc-1bkq2us-0 eWXbsW">
															</div>
														</div>
													</div>
													<div class="Box-sc-5vx4ls-0 jiMkSI">
														<div data-state="closed">
															<div aria-controls="radix-id-2322785538-4632"
																aria-expanded="false" data-state="closed"
																class="Box-sc-5vx4ls-0 cGOgLs Trigger__CollapsibleTrigger-sc-zrl3ha-0 HBTNX">
																<div display="flex"
																	class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 jnDyMP kqsqjK NavigationTree__StyledFlex-sc-1f9wbbd-1 bktzmf">
																	<div class="Box-sc-5vx4ls-0 hZRMgn"><svg width="12"
																			height="12" viewBox="0 0 24 24" fill="none"
																			xmlns="http://www.w3.org/2000/svg">
																			<path fill-rule="evenodd"
																				clip-rule="evenodd"
																				d="M8.293 5.293a1 1 0 0 1 1.414 0l6 6a1 1 0 0 1 0 1.414l-6 6a1 1 0 0 1-1.414-1.414L13.586 12 8.293 6.707a1 1 0 0 1 0-1.414Z"
																				fill="hsla(214, 18%, 69%, 1)"></path>
																		</svg></div>
																	<p
																		class="Text-sc-1g8cvhx-0 NavigationTree__NavNodeCollapsibleTriggerText-sc-1f9wbbd-2 HSevc gknCtx">
																		WHMCS</p>
																</div>
															</div>
															<div data-state="closed" id="radix-id-2322785538-4632"
																hidden=""
																class="Content__CollapsibleContent-sc-1bkq2us-0 eWXbsW">
															</div>
														</div>
													</div>
													<div class="Box-sc-5vx4ls-0 jiMkSI">
														<div data-state="closed">
															<div aria-controls="radix-id-2322785538-4633"
																aria-expanded="false" data-state="closed"
																class="Box-sc-5vx4ls-0 cGOgLs Trigger__CollapsibleTrigger-sc-zrl3ha-0 HBTNX">
																<div display="flex"
																	class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 jnDyMP kqsqjK NavigationTree__StyledFlex-sc-1f9wbbd-1 bktzmf">
																	<div class="Box-sc-5vx4ls-0 hZRMgn"><svg width="12"
																			height="12" viewBox="0 0 24 24" fill="none"
																			xmlns="http://www.w3.org/2000/svg">
																			<path fill-rule="evenodd"
																				clip-rule="evenodd"
																				d="M8.293 5.293a1 1 0 0 1 1.414 0l6 6a1 1 0 0 1 0 1.414l-6 6a1 1 0 0 1-1.414-1.414L13.586 12 8.293 6.707a1 1 0 0 1 0-1.414Z"
																				fill="hsla(214, 18%, 69%, 1)"></path>
																		</svg></div>
																	<p
																		class="Text-sc-1g8cvhx-0 NavigationTree__NavNodeCollapsibleTriggerText-sc-1f9wbbd-2 HSevc gknCtx">
																		Wix</p>
																</div>
															</div>
															<div data-state="closed" id="radix-id-2322785538-4633"
																hidden=""
																class="Content__CollapsibleContent-sc-1bkq2us-0 eWXbsW">
															</div>
														</div>
													</div>
													<div class="Box-sc-5vx4ls-0 jiMkSI">
														<div data-state="closed">
															<div aria-controls="radix-id-2322785538-4634"
																aria-expanded="false" data-state="closed"
																class="Box-sc-5vx4ls-0 cGOgLs Trigger__CollapsibleTrigger-sc-zrl3ha-0 HBTNX">
																<div display="flex"
																	class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 jnDyMP kqsqjK NavigationTree__StyledFlex-sc-1f9wbbd-1 bktzmf">
																	<div class="Box-sc-5vx4ls-0 hZRMgn"><svg width="12"
																			height="12" viewBox="0 0 24 24" fill="none"
																			xmlns="http://www.w3.org/2000/svg">
																			<path fill-rule="evenodd"
																				clip-rule="evenodd"
																				d="M8.293 5.293a1 1 0 0 1 1.414 0l6 6a1 1 0 0 1 0 1.414l-6 6a1 1 0 0 1-1.414-1.414L13.586 12 8.293 6.707a1 1 0 0 1 0-1.414Z"
																				fill="hsla(214, 18%, 69%, 1)"></path>
																		</svg></div>
																	<p
																		class="Text-sc-1g8cvhx-0 NavigationTree__NavNodeCollapsibleTriggerText-sc-1f9wbbd-2 HSevc gknCtx">
																		Woocommerce</p>
																</div>
															</div>
															<div data-state="closed" id="radix-id-2322785538-4634"
																hidden=""
																class="Content__CollapsibleContent-sc-1bkq2us-0 eWXbsW">
															</div>
														</div>
													</div>
													<div class="Box-sc-5vx4ls-0 jiMkSI">
														<div data-state="closed">
															<div aria-controls="radix-id-2322785538-4635"
																aria-expanded="false" data-state="closed"
																class="Box-sc-5vx4ls-0 cGOgLs Trigger__CollapsibleTrigger-sc-zrl3ha-0 HBTNX">
																<div display="flex"
																	class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 jnDyMP kqsqjK NavigationTree__StyledFlex-sc-1f9wbbd-1 bktzmf">
																	<div class="Box-sc-5vx4ls-0 hZRMgn"><svg width="12"
																			height="12" viewBox="0 0 24 24" fill="none"
																			xmlns="http://www.w3.org/2000/svg">
																			<path fill-rule="evenodd"
																				clip-rule="evenodd"
																				d="M8.293 5.293a1 1 0 0 1 1.414 0l6 6a1 1 0 0 1 0 1.414l-6 6a1 1 0 0 1-1.414-1.414L13.586 12 8.293 6.707a1 1 0 0 1 0-1.414Z"
																				fill="hsla(214, 18%, 69%, 1)"></path>
																		</svg></div>
																	<p
																		class="Text-sc-1g8cvhx-0 NavigationTree__NavNodeCollapsibleTriggerText-sc-1f9wbbd-2 HSevc gknCtx">
																		WordPress</p>
																</div>
															</div>
															<div data-state="closed" id="radix-id-2322785538-4635"
																hidden=""
																class="Content__CollapsibleContent-sc-1bkq2us-0 eWXbsW">
															</div>
														</div>
													</div>
												</nav>
											</div>
										</div>
									</div>
								</div>
							</div>
							<div class="Box-sc-5vx4ls-0 jiMkSI">
								<div data-state="closed">
									<div aria-controls="radix-id-2322785538-4636" aria-expanded="false"
										data-state="closed"
										class="Box-sc-5vx4ls-0 cGOgLs Trigger__CollapsibleTrigger-sc-zrl3ha-0 HBTNX">
										<div display="flex"
											class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 jnDyMP kqsqjK NavigationTree__StyledFlex-sc-1f9wbbd-1 bktzmf">
											<div class="Box-sc-5vx4ls-0 hZRMgn"><svg width="12" height="12"
													viewBox="0 0 10 8" fill="none" xmlns="http://www.w3.org/2000/svg"
													data-testid="double-chevron-right">
													<path
														d="M1.21936 0.195262C0.940416 -0.0650874 0.488155 -0.0650874 0.209209 0.195262C-0.0697365 0.455612 -0.0697365 0.877722 0.209209 1.13807L3.27556 4L0.209209 6.86193C-0.0697365 7.12228 -0.0697365 7.54439 0.209209 7.80474C0.488155 8.06509 0.940416 8.06509 1.21936 7.80474L4.79079 4.4714C5.06974 4.21106 5.06974 3.78894 4.79079 3.5286L1.21936 0.195262Z"
														fill="hsla(214, 18%, 69%, 1)"></path>
													<path
														d="M6.21936 0.195262C5.94042 -0.0650874 5.48816 -0.0650874 5.20921 0.195262C4.93026 0.455612 4.93026 0.877722 5.20921 1.13807L8.27556 4L5.20921 6.86193C4.93026 7.12228 4.93026 7.54439 5.20921 7.80474C5.48816 8.06509 5.94042 8.06509 6.21936 7.80474L9.79079 4.4714C10.0697 4.21106 10.0697 3.78894 9.79079 3.5286L6.21936 0.195262Z"
														fill="hsla(214, 18%, 69%, 1)"></path>
												</svg></div>
											<p
												class="Text-sc-1g8cvhx-0 NavigationTree__NavNodeCollapsibleTriggerText-sc-1f9wbbd-2 HSevc coZHyU">
												Magic Checkout</p>
										</div>
									</div>
									<div data-state="closed" id="radix-id-2322785538-4636" hidden=""
										class="Content__CollapsibleContent-sc-1bkq2us-0 eWXbsW"></div>
								</div>
							</div>
							<div class="Box-sc-5vx4ls-0 jiMkSI">
								<div data-state="closed">
									<div aria-controls="radix-id-2322785538-4637" aria-expanded="false"
										data-state="closed"
										class="Box-sc-5vx4ls-0 cGOgLs Trigger__CollapsibleTrigger-sc-zrl3ha-0 HBTNX">
										<div display="flex"
											class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 jnDyMP kqsqjK NavigationTree__StyledFlex-sc-1f9wbbd-1 bktzmf">
											<div class="Box-sc-5vx4ls-0 hZRMgn"><svg width="12" height="12"
													viewBox="0 0 10 8" fill="none" xmlns="http://www.w3.org/2000/svg"
													data-testid="double-chevron-right">
													<path
														d="M1.21936 0.195262C0.940416 -0.0650874 0.488155 -0.0650874 0.209209 0.195262C-0.0697365 0.455612 -0.0697365 0.877722 0.209209 1.13807L3.27556 4L0.209209 6.86193C-0.0697365 7.12228 -0.0697365 7.54439 0.209209 7.80474C0.488155 8.06509 0.940416 8.06509 1.21936 7.80474L4.79079 4.4714C5.06974 4.21106 5.06974 3.78894 4.79079 3.5286L1.21936 0.195262Z"
														fill="hsla(214, 18%, 69%, 1)"></path>
													<path
														d="M6.21936 0.195262C5.94042 -0.0650874 5.48816 -0.0650874 5.20921 0.195262C4.93026 0.455612 4.93026 0.877722 5.20921 1.13807L8.27556 4L5.20921 6.86193C4.93026 7.12228 4.93026 7.54439 5.20921 7.80474C5.48816 8.06509 5.94042 8.06509 6.21936 7.80474L9.79079 4.4714C10.0697 4.21106 10.0697 3.78894 9.79079 3.5286L6.21936 0.195262Z"
														fill="hsla(214, 18%, 69%, 1)"></path>
												</svg></div>
											<p
												class="Text-sc-1g8cvhx-0 NavigationTree__NavNodeCollapsibleTriggerText-sc-1f9wbbd-2 HSevc coZHyU">
												Payment Links</p>
										</div>
									</div>
									<div data-state="closed" id="radix-id-2322785538-4637" hidden=""
										class="Content__CollapsibleContent-sc-1bkq2us-0 eWXbsW"></div>
								</div>
							</div>
							<div class="Box-sc-5vx4ls-0 jiMkSI">
								<div data-state="closed">
									<div aria-controls="radix-id-2322785538-4638" aria-expanded="false"
										data-state="closed"
										class="Box-sc-5vx4ls-0 cGOgLs Trigger__CollapsibleTrigger-sc-zrl3ha-0 HBTNX">
										<div display="flex"
											class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 jnDyMP kqsqjK NavigationTree__StyledFlex-sc-1f9wbbd-1 bktzmf">
											<div class="Box-sc-5vx4ls-0 hZRMgn"><svg width="12" height="12"
													viewBox="0 0 10 8" fill="none" xmlns="http://www.w3.org/2000/svg"
													data-testid="double-chevron-right">
													<path
														d="M1.21936 0.195262C0.940416 -0.0650874 0.488155 -0.0650874 0.209209 0.195262C-0.0697365 0.455612 -0.0697365 0.877722 0.209209 1.13807L3.27556 4L0.209209 6.86193C-0.0697365 7.12228 -0.0697365 7.54439 0.209209 7.80474C0.488155 8.06509 0.940416 8.06509 1.21936 7.80474L4.79079 4.4714C5.06974 4.21106 5.06974 3.78894 4.79079 3.5286L1.21936 0.195262Z"
														fill="hsla(214, 18%, 69%, 1)"></path>
													<path
														d="M6.21936 0.195262C5.94042 -0.0650874 5.48816 -0.0650874 5.20921 0.195262C4.93026 0.455612 4.93026 0.877722 5.20921 1.13807L8.27556 4L5.20921 6.86193C4.93026 7.12228 4.93026 7.54439 5.20921 7.80474C5.48816 8.06509 5.94042 8.06509 6.21936 7.80474L9.79079 4.4714C10.0697 4.21106 10.0697 3.78894 9.79079 3.5286L6.21936 0.195262Z"
														fill="hsla(214, 18%, 69%, 1)"></path>
												</svg></div>
											<p
												class="Text-sc-1g8cvhx-0 NavigationTree__NavNodeCollapsibleTriggerText-sc-1f9wbbd-2 HSevc coZHyU">
												Payment Button</p>
										</div>
									</div>
									<div data-state="closed" id="radix-id-2322785538-4638" hidden=""
										class="Content__CollapsibleContent-sc-1bkq2us-0 eWXbsW"></div>
								</div>
							</div>
							<div class="Box-sc-5vx4ls-0 jiMkSI">
								<div data-state="closed">
									<div aria-controls="radix-id-2322785538-4639" aria-expanded="false"
										data-state="closed"
										class="Box-sc-5vx4ls-0 cGOgLs Trigger__CollapsibleTrigger-sc-zrl3ha-0 HBTNX">
										<div display="flex"
											class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 jnDyMP kqsqjK NavigationTree__StyledFlex-sc-1f9wbbd-1 bktzmf">
											<div class="Box-sc-5vx4ls-0 hZRMgn"><svg width="12" height="12"
													viewBox="0 0 10 8" fill="none" xmlns="http://www.w3.org/2000/svg"
													data-testid="double-chevron-right">
													<path
														d="M1.21936 0.195262C0.940416 -0.0650874 0.488155 -0.0650874 0.209209 0.195262C-0.0697365 0.455612 -0.0697365 0.877722 0.209209 1.13807L3.27556 4L0.209209 6.86193C-0.0697365 7.12228 -0.0697365 7.54439 0.209209 7.80474C0.488155 8.06509 0.940416 8.06509 1.21936 7.80474L4.79079 4.4714C5.06974 4.21106 5.06974 3.78894 4.79079 3.5286L1.21936 0.195262Z"
														fill="hsla(214, 18%, 69%, 1)"></path>
													<path
														d="M6.21936 0.195262C5.94042 -0.0650874 5.48816 -0.0650874 5.20921 0.195262C4.93026 0.455612 4.93026 0.877722 5.20921 1.13807L8.27556 4L5.20921 6.86193C4.93026 7.12228 4.93026 7.54439 5.20921 7.80474C5.48816 8.06509 5.94042 8.06509 6.21936 7.80474L9.79079 4.4714C10.0697 4.21106 10.0697 3.78894 9.79079 3.5286L6.21936 0.195262Z"
														fill="hsla(214, 18%, 69%, 1)"></path>
												</svg></div>
											<p
												class="Text-sc-1g8cvhx-0 NavigationTree__NavNodeCollapsibleTriggerText-sc-1f9wbbd-2 HSevc coZHyU">
												Payment Pages</p>
										</div>
									</div>
									<div data-state="closed" id="radix-id-2322785538-4639" hidden=""
										class="Content__CollapsibleContent-sc-1bkq2us-0 eWXbsW"></div>
								</div>
							</div>
							<div class="Box-sc-5vx4ls-0 jiMkSI">
								<div data-state="closed">
									<div aria-controls="radix-id-2322785538-4640" aria-expanded="false"
										data-state="closed"
										class="Box-sc-5vx4ls-0 cGOgLs Trigger__CollapsibleTrigger-sc-zrl3ha-0 HBTNX">
										<div display="flex"
											class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 jnDyMP kqsqjK NavigationTree__StyledFlex-sc-1f9wbbd-1 bktzmf">
											<div class="Box-sc-5vx4ls-0 hZRMgn"><svg width="12" height="12"
													viewBox="0 0 10 8" fill="none" xmlns="http://www.w3.org/2000/svg"
													data-testid="double-chevron-right">
													<path
														d="M1.21936 0.195262C0.940416 -0.0650874 0.488155 -0.0650874 0.209209 0.195262C-0.0697365 0.455612 -0.0697365 0.877722 0.209209 1.13807L3.27556 4L0.209209 6.86193C-0.0697365 7.12228 -0.0697365 7.54439 0.209209 7.80474C0.488155 8.06509 0.940416 8.06509 1.21936 7.80474L4.79079 4.4714C5.06974 4.21106 5.06974 3.78894 4.79079 3.5286L1.21936 0.195262Z"
														fill="hsla(214, 18%, 69%, 1)"></path>
													<path
														d="M6.21936 0.195262C5.94042 -0.0650874 5.48816 -0.0650874 5.20921 0.195262C4.93026 0.455612 4.93026 0.877722 5.20921 1.13807L8.27556 4L5.20921 6.86193C4.93026 7.12228 4.93026 7.54439 5.20921 7.80474C5.48816 8.06509 5.94042 8.06509 6.21936 7.80474L9.79079 4.4714C10.0697 4.21106 10.0697 3.78894 9.79079 3.5286L6.21936 0.195262Z"
														fill="hsla(214, 18%, 69%, 1)"></path>
												</svg></div>
											<p
												class="Text-sc-1g8cvhx-0 NavigationTree__NavNodeCollapsibleTriggerText-sc-1f9wbbd-2 HSevc coZHyU">
												Invoices</p>
										</div>
									</div>
									<div data-state="closed" id="radix-id-2322785538-4640" hidden=""
										class="Content__CollapsibleContent-sc-1bkq2us-0 eWXbsW"></div>
								</div>
							</div>
							<div class="Box-sc-5vx4ls-0 jiMkSI">
								<div data-state="closed">
									<div aria-controls="radix-id-2322785538-4641" aria-expanded="false"
										data-state="closed"
										class="Box-sc-5vx4ls-0 cGOgLs Trigger__CollapsibleTrigger-sc-zrl3ha-0 HBTNX">
										<div display="flex"
											class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 jnDyMP kqsqjK NavigationTree__StyledFlex-sc-1f9wbbd-1 bktzmf">
											<div class="Box-sc-5vx4ls-0 hZRMgn"><svg width="12" height="12"
													viewBox="0 0 10 8" fill="none" xmlns="http://www.w3.org/2000/svg"
													data-testid="double-chevron-right">
													<path
														d="M1.21936 0.195262C0.940416 -0.0650874 0.488155 -0.0650874 0.209209 0.195262C-0.0697365 0.455612 -0.0697365 0.877722 0.209209 1.13807L3.27556 4L0.209209 6.86193C-0.0697365 7.12228 -0.0697365 7.54439 0.209209 7.80474C0.488155 8.06509 0.940416 8.06509 1.21936 7.80474L4.79079 4.4714C5.06974 4.21106 5.06974 3.78894 4.79079 3.5286L1.21936 0.195262Z"
														fill="hsla(214, 18%, 69%, 1)"></path>
													<path
														d="M6.21936 0.195262C5.94042 -0.0650874 5.48816 -0.0650874 5.20921 0.195262C4.93026 0.455612 4.93026 0.877722 5.20921 1.13807L8.27556 4L5.20921 6.86193C4.93026 7.12228 4.93026 7.54439 5.20921 7.80474C5.48816 8.06509 5.94042 8.06509 6.21936 7.80474L9.79079 4.4714C10.0697 4.21106 10.0697 3.78894 9.79079 3.5286L6.21936 0.195262Z"
														fill="hsla(214, 18%, 69%, 1)"></path>
												</svg></div>
											<p
												class="Text-sc-1g8cvhx-0 NavigationTree__NavNodeCollapsibleTriggerText-sc-1f9wbbd-2 HSevc coZHyU">
												QR Codes</p>
										</div>
									</div>
									<div data-state="closed" id="radix-id-2322785538-4641" hidden=""
										class="Content__CollapsibleContent-sc-1bkq2us-0 eWXbsW"></div>
								</div>
							</div>
							<div class="Box-sc-5vx4ls-0 jiMkSI">
								<div data-state="closed">
									<div aria-controls="radix-id-2322785538-4642" aria-expanded="false"
										data-state="closed"
										class="Box-sc-5vx4ls-0 cGOgLs Trigger__CollapsibleTrigger-sc-zrl3ha-0 HBTNX">
										<div display="flex"
											class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 jnDyMP kqsqjK NavigationTree__StyledFlex-sc-1f9wbbd-1 bktzmf">
											<div class="Box-sc-5vx4ls-0 hZRMgn"><svg width="12" height="12"
													viewBox="0 0 10 8" fill="none" xmlns="http://www.w3.org/2000/svg"
													data-testid="double-chevron-right">
													<path
														d="M1.21936 0.195262C0.940416 -0.0650874 0.488155 -0.0650874 0.209209 0.195262C-0.0697365 0.455612 -0.0697365 0.877722 0.209209 1.13807L3.27556 4L0.209209 6.86193C-0.0697365 7.12228 -0.0697365 7.54439 0.209209 7.80474C0.488155 8.06509 0.940416 8.06509 1.21936 7.80474L4.79079 4.4714C5.06974 4.21106 5.06974 3.78894 4.79079 3.5286L1.21936 0.195262Z"
														fill="hsla(214, 18%, 69%, 1)"></path>
													<path
														d="M6.21936 0.195262C5.94042 -0.0650874 5.48816 -0.0650874 5.20921 0.195262C4.93026 0.455612 4.93026 0.877722 5.20921 1.13807L8.27556 4L5.20921 6.86193C4.93026 7.12228 4.93026 7.54439 5.20921 7.80474C5.48816 8.06509 5.94042 8.06509 6.21936 7.80474L9.79079 4.4714C10.0697 4.21106 10.0697 3.78894 9.79079 3.5286L6.21936 0.195262Z"
														fill="hsla(214, 18%, 69%, 1)"></path>
												</svg></div>
											<p
												class="Text-sc-1g8cvhx-0 NavigationTree__NavNodeCollapsibleTriggerText-sc-1f9wbbd-2 HSevc coZHyU">
												Affordability</p>
										</div>
									</div>
									<div data-state="closed" id="radix-id-2322785538-4642" hidden=""
										class="Content__CollapsibleContent-sc-1bkq2us-0 eWXbsW"></div>
								</div>
							</div>
							<div class="Box-sc-5vx4ls-0 jiMkSI">
								<div data-state="closed">
									<div aria-controls="radix-id-2322785538-4643" aria-expanded="false"
										data-state="closed"
										class="Box-sc-5vx4ls-0 cGOgLs Trigger__CollapsibleTrigger-sc-zrl3ha-0 HBTNX">
										<div display="flex"
											class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 jnDyMP kqsqjK NavigationTree__StyledFlex-sc-1f9wbbd-1 bktzmf">
											<div class="Box-sc-5vx4ls-0 hZRMgn"><svg width="12" height="12"
													viewBox="0 0 10 8" fill="none" xmlns="http://www.w3.org/2000/svg"
													data-testid="double-chevron-right">
													<path
														d="M1.21936 0.195262C0.940416 -0.0650874 0.488155 -0.0650874 0.209209 0.195262C-0.0697365 0.455612 -0.0697365 0.877722 0.209209 1.13807L3.27556 4L0.209209 6.86193C-0.0697365 7.12228 -0.0697365 7.54439 0.209209 7.80474C0.488155 8.06509 0.940416 8.06509 1.21936 7.80474L4.79079 4.4714C5.06974 4.21106 5.06974 3.78894 4.79079 3.5286L1.21936 0.195262Z"
														fill="hsla(214, 18%, 69%, 1)"></path>
													<path
														d="M6.21936 0.195262C5.94042 -0.0650874 5.48816 -0.0650874 5.20921 0.195262C4.93026 0.455612 4.93026 0.877722 5.20921 1.13807L8.27556 4L5.20921 6.86193C4.93026 7.12228 4.93026 7.54439 5.20921 7.80474C5.48816 8.06509 5.94042 8.06509 6.21936 7.80474L9.79079 4.4714C10.0697 4.21106 10.0697 3.78894 9.79079 3.5286L6.21936 0.195262Z"
														fill="hsla(214, 18%, 69%, 1)"></path>
												</svg></div>
											<p
												class="Text-sc-1g8cvhx-0 NavigationTree__NavNodeCollapsibleTriggerText-sc-1f9wbbd-2 HSevc coZHyU">
												Subscriptions</p>
										</div>
									</div>
									<div data-state="closed" id="radix-id-2322785538-4643" hidden=""
										class="Content__CollapsibleContent-sc-1bkq2us-0 eWXbsW"></div>
								</div>
							</div>
							<div class="Box-sc-5vx4ls-0 jiMkSI">
								<div data-state="closed">
									<div aria-controls="radix-id-2322785538-4644" aria-expanded="false"
										data-state="closed"
										class="Box-sc-5vx4ls-0 cGOgLs Trigger__CollapsibleTrigger-sc-zrl3ha-0 HBTNX">
										<div display="flex"
											class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 jnDyMP kqsqjK NavigationTree__StyledFlex-sc-1f9wbbd-1 bktzmf">
											<div class="Box-sc-5vx4ls-0 hZRMgn"><svg width="12" height="12"
													viewBox="0 0 10 8" fill="none" xmlns="http://www.w3.org/2000/svg"
													data-testid="double-chevron-right">
													<path
														d="M1.21936 0.195262C0.940416 -0.0650874 0.488155 -0.0650874 0.209209 0.195262C-0.0697365 0.455612 -0.0697365 0.877722 0.209209 1.13807L3.27556 4L0.209209 6.86193C-0.0697365 7.12228 -0.0697365 7.54439 0.209209 7.80474C0.488155 8.06509 0.940416 8.06509 1.21936 7.80474L4.79079 4.4714C5.06974 4.21106 5.06974 3.78894 4.79079 3.5286L1.21936 0.195262Z"
														fill="hsla(214, 18%, 69%, 1)"></path>
													<path
														d="M6.21936 0.195262C5.94042 -0.0650874 5.48816 -0.0650874 5.20921 0.195262C4.93026 0.455612 4.93026 0.877722 5.20921 1.13807L8.27556 4L5.20921 6.86193C4.93026 7.12228 4.93026 7.54439 5.20921 7.80474C5.48816 8.06509 5.94042 8.06509 6.21936 7.80474L9.79079 4.4714C10.0697 4.21106 10.0697 3.78894 9.79079 3.5286L6.21936 0.195262Z"
														fill="hsla(214, 18%, 69%, 1)"></path>
												</svg></div>
											<p
												class="Text-sc-1g8cvhx-0 NavigationTree__NavNodeCollapsibleTriggerText-sc-1f9wbbd-2 HSevc coZHyU">
												Smart Collect</p>
										</div>
									</div>
									<div data-state="closed" id="radix-id-2322785538-4644" hidden=""
										class="Content__CollapsibleContent-sc-1bkq2us-0 eWXbsW"></div>
								</div>
							</div>
							<div class="Box-sc-5vx4ls-0 jiMkSI">
								<div data-state="closed">
									<div aria-controls="radix-id-2322785538-4645" aria-expanded="false"
										data-state="closed"
										class="Box-sc-5vx4ls-0 cGOgLs Trigger__CollapsibleTrigger-sc-zrl3ha-0 HBTNX">
										<div display="flex"
											class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 jnDyMP kqsqjK NavigationTree__StyledFlex-sc-1f9wbbd-1 bktzmf">
											<div class="Box-sc-5vx4ls-0 hZRMgn"><svg width="12" height="12"
													viewBox="0 0 10 8" fill="none" xmlns="http://www.w3.org/2000/svg"
													data-testid="double-chevron-right">
													<path
														d="M1.21936 0.195262C0.940416 -0.0650874 0.488155 -0.0650874 0.209209 0.195262C-0.0697365 0.455612 -0.0697365 0.877722 0.209209 1.13807L3.27556 4L0.209209 6.86193C-0.0697365 7.12228 -0.0697365 7.54439 0.209209 7.80474C0.488155 8.06509 0.940416 8.06509 1.21936 7.80474L4.79079 4.4714C5.06974 4.21106 5.06974 3.78894 4.79079 3.5286L1.21936 0.195262Z"
														fill="hsla(214, 18%, 69%, 1)"></path>
													<path
														d="M6.21936 0.195262C5.94042 -0.0650874 5.48816 -0.0650874 5.20921 0.195262C4.93026 0.455612 4.93026 0.877722 5.20921 1.13807L8.27556 4L5.20921 6.86193C4.93026 7.12228 4.93026 7.54439 5.20921 7.80474C5.48816 8.06509 5.94042 8.06509 6.21936 7.80474L9.79079 4.4714C10.0697 4.21106 10.0697 3.78894 9.79079 3.5286L6.21936 0.195262Z"
														fill="hsla(214, 18%, 69%, 1)"></path>
												</svg></div>
											<p
												class="Text-sc-1g8cvhx-0 NavigationTree__NavNodeCollapsibleTriggerText-sc-1f9wbbd-2 HSevc coZHyU">
												Optimizer</p>
										</div>
									</div>
									<div data-state="closed" id="radix-id-2322785538-4645" hidden=""
										class="Content__CollapsibleContent-sc-1bkq2us-0 eWXbsW"></div>
								</div>
							</div>
							<div class="Box-sc-5vx4ls-0 jiMkSI">
								<div data-state="closed">
									<div aria-controls="radix-id-2322785538-4646" aria-expanded="false"
										data-state="closed"
										class="Box-sc-5vx4ls-0 cGOgLs Trigger__CollapsibleTrigger-sc-zrl3ha-0 HBTNX">
										<div display="flex"
											class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 jnDyMP kqsqjK NavigationTree__StyledFlex-sc-1f9wbbd-1 bktzmf">
											<div class="Box-sc-5vx4ls-0 hZRMgn"><svg width="12" height="12"
													viewBox="0 0 10 8" fill="none" xmlns="http://www.w3.org/2000/svg"
													data-testid="double-chevron-right">
													<path
														d="M1.21936 0.195262C0.940416 -0.0650874 0.488155 -0.0650874 0.209209 0.195262C-0.0697365 0.455612 -0.0697365 0.877722 0.209209 1.13807L3.27556 4L0.209209 6.86193C-0.0697365 7.12228 -0.0697365 7.54439 0.209209 7.80474C0.488155 8.06509 0.940416 8.06509 1.21936 7.80474L4.79079 4.4714C5.06974 4.21106 5.06974 3.78894 4.79079 3.5286L1.21936 0.195262Z"
														fill="hsla(214, 18%, 69%, 1)"></path>
													<path
														d="M6.21936 0.195262C5.94042 -0.0650874 5.48816 -0.0650874 5.20921 0.195262C4.93026 0.455612 4.93026 0.877722 5.20921 1.13807L8.27556 4L5.20921 6.86193C4.93026 7.12228 4.93026 7.54439 5.20921 7.80474C5.48816 8.06509 5.94042 8.06509 6.21936 7.80474L9.79079 4.4714C10.0697 4.21106 10.0697 3.78894 9.79079 3.5286L6.21936 0.195262Z"
														fill="hsla(214, 18%, 69%, 1)"></path>
												</svg></div>
											<p
												class="Text-sc-1g8cvhx-0 NavigationTree__NavNodeCollapsibleTriggerText-sc-1f9wbbd-2 HSevc coZHyU">
												Route</p>
										</div>
									</div>
									<div data-state="closed" id="radix-id-2322785538-4646" hidden=""
										class="Content__CollapsibleContent-sc-1bkq2us-0 eWXbsW"></div>
								</div>
							</div>
							<div class="Box-sc-5vx4ls-0 jiMkSI">
								<div data-state="closed">
									<div aria-controls="radix-id-2322785538-4647" aria-expanded="false"
										data-state="closed"
										class="Box-sc-5vx4ls-0 cGOgLs Trigger__CollapsibleTrigger-sc-zrl3ha-0 HBTNX">
										<div display="flex"
											class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 jnDyMP kqsqjK NavigationTree__StyledFlex-sc-1f9wbbd-1 bktzmf">
											<div class="Box-sc-5vx4ls-0 hZRMgn"><svg width="12" height="12"
													viewBox="0 0 10 8" fill="none" xmlns="http://www.w3.org/2000/svg"
													data-testid="double-chevron-right">
													<path
														d="M1.21936 0.195262C0.940416 -0.0650874 0.488155 -0.0650874 0.209209 0.195262C-0.0697365 0.455612 -0.0697365 0.877722 0.209209 1.13807L3.27556 4L0.209209 6.86193C-0.0697365 7.12228 -0.0697365 7.54439 0.209209 7.80474C0.488155 8.06509 0.940416 8.06509 1.21936 7.80474L4.79079 4.4714C5.06974 4.21106 5.06974 3.78894 4.79079 3.5286L1.21936 0.195262Z"
														fill="hsla(214, 18%, 69%, 1)"></path>
													<path
														d="M6.21936 0.195262C5.94042 -0.0650874 5.48816 -0.0650874 5.20921 0.195262C4.93026 0.455612 4.93026 0.877722 5.20921 1.13807L8.27556 4L5.20921 6.86193C4.93026 7.12228 4.93026 7.54439 5.20921 7.80474C5.48816 8.06509 5.94042 8.06509 6.21936 7.80474L9.79079 4.4714C10.0697 4.21106 10.0697 3.78894 9.79079 3.5286L6.21936 0.195262Z"
														fill="hsla(214, 18%, 69%, 1)"></path>
												</svg></div>
											<p
												class="Text-sc-1g8cvhx-0 NavigationTree__NavNodeCollapsibleTriggerText-sc-1f9wbbd-2 HSevc coZHyU">
												Third Party Validation</p>
										</div>
									</div>
									<div data-state="closed" id="radix-id-2322785538-4647" hidden=""
										class="Content__CollapsibleContent-sc-1bkq2us-0 eWXbsW"></div>
								</div>
							</div>
							<div class="Box-sc-5vx4ls-0 jiMkSI">
								<div data-state="closed">
									<div aria-controls="radix-id-2322785538-4648" aria-expanded="false"
										data-state="closed"
										class="Box-sc-5vx4ls-0 cGOgLs Trigger__CollapsibleTrigger-sc-zrl3ha-0 HBTNX">
										<div display="flex"
											class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 jnDyMP kqsqjK NavigationTree__StyledFlex-sc-1f9wbbd-1 bktzmf">
											<div class="Box-sc-5vx4ls-0 hZRMgn"><svg width="12" height="12"
													viewBox="0 0 10 8" fill="none" xmlns="http://www.w3.org/2000/svg"
													data-testid="double-chevron-right">
													<path
														d="M1.21936 0.195262C0.940416 -0.0650874 0.488155 -0.0650874 0.209209 0.195262C-0.0697365 0.455612 -0.0697365 0.877722 0.209209 1.13807L3.27556 4L0.209209 6.86193C-0.0697365 7.12228 -0.0697365 7.54439 0.209209 7.80474C0.488155 8.06509 0.940416 8.06509 1.21936 7.80474L4.79079 4.4714C5.06974 4.21106 5.06974 3.78894 4.79079 3.5286L1.21936 0.195262Z"
														fill="hsla(214, 18%, 69%, 1)"></path>
													<path
														d="M6.21936 0.195262C5.94042 -0.0650874 5.48816 -0.0650874 5.20921 0.195262C4.93026 0.455612 4.93026 0.877722 5.20921 1.13807L8.27556 4L5.20921 6.86193C4.93026 7.12228 4.93026 7.54439 5.20921 7.80474C5.48816 8.06509 5.94042 8.06509 6.21936 7.80474L9.79079 4.4714C10.0697 4.21106 10.0697 3.78894 9.79079 3.5286L6.21936 0.195262Z"
														fill="hsla(214, 18%, 69%, 1)"></path>
												</svg></div>
											<p
												class="Text-sc-1g8cvhx-0 NavigationTree__NavNodeCollapsibleTriggerText-sc-1f9wbbd-2 HSevc coZHyU">
												Payments Mobile App</p>
										</div>
									</div>
									<div data-state="closed" id="radix-id-2322785538-4648" hidden=""
										class="Content__CollapsibleContent-sc-1bkq2us-0 eWXbsW"></div>
								</div>
							</div>
							<div
								class="Box-sc-5vx4ls-0 SidebarNavLink__SidebarnavLinkContainer-sc-pt5di4-0 bQnGvS fWgtQP">
								<div display="flex"
									class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 dPVYbu fCPAWO Link__StyledLink-sc-38tiy-0 kWnpZi">
									<a id="payments/epos-app-sidebar" target="_self"
										href="/docs/payments/epos-app"><span class="Text-sc-1g8cvhx-0 SidebarNavLink__SidebarnavLinkText-sc-pt5di4-1 bsHdmV kVxEKo">ePOS App (Deprecated)</span></a>
								</div>
							</div>
							<div
								class="Box-sc-5vx4ls-0 SidebarNavLink__SidebarnavLinkContainer-sc-pt5di4-0 bQnGvS fWgtQP">
								<div display="flex"
									class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 dPVYbu fCPAWO Link__StyledLink-sc-38tiy-0 kWnpZi">
									<a id="payments/thirdwatch-sidebar" target="_self"
										href="/docs/payments/thirdwatch"><span class="Text-sc-1g8cvhx-0 SidebarNavLink__SidebarnavLinkText-sc-pt5di4-1 bsHdmV kVxEKo">Thirdwatch (Deprecated)</span></a>
								</div>
							</div>
							<div
								class="Box-sc-5vx4ls-0 SidebarNavLink__SidebarnavLinkContainer-sc-pt5di4-0 bQnGvS fWgtQP">
								<div display="flex"
									class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 dPVYbu fCPAWO Link__StyledLink-sc-38tiy-0 kWnpZi">
									<a id="payments/glossary-sidebar" target="_self"
										href="/docs/payments/glossary"><span class="Text-sc-1g8cvhx-0 SidebarNavLink__SidebarnavLinkText-sc-pt5di4-1 bsHdmV kVxEKo">Glossary</span></a>
								</div>
							</div>
						</nav>
					</nav>
				</div>
				<div display="flex" width="calc(100% - 328px)"
					class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 iANuVs gyXFoV">
					<div id="banner-root" style="position:sticky;top:56px;z-index:1"></div>
					<div display="flex" id="content" width="100%"
						class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 dGChSs ekisLk">
						<div display="flex"
							class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 NWmfY fwnSqg layout-product"
							width="[object Object]">
							<div class="Box-sc-5vx4ls-0 dWYgks">
								<div display="flex" data-testid="breadcrumbs-container"
									class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 ldkSSq fCPAWO styled__StyledBreadcrumbsContainer-sc-mcrmsw-0 bjYPIl">
									<div display="flex"
										class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 gbWiaG fCPAWO Link__StyledLink-sc-38tiy-0 kWnpZi">
										<a id="breadcrumb-0" target="_self" href="/docs/payments">
											<p class="Text-sc-1g8cvhx-0 Link__StyledText-sc-38tiy-2 ifSOxV SCkGc">
												Payments</p>
										</a></div>
									<div display="flex"
										class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 gbWiaG fCPAWO Link__StyledLink-sc-38tiy-0 kWnpZi">
										<a id="breadcrumb-1" target="_self" href="/docs/payments/payment-gateway">
											<p class="Text-sc-1g8cvhx-0 Link__StyledText-sc-38tiy-2 ifSOxV SCkGc">
												Payment Gateway</p>
										</a></div>
									<div display="flex" id="breadcrumb-2"
										class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 gbWiaG fCPAWO styled__StyledTextContainer-sc-mcrmsw-1 fsUibx">
										<p class="Text-sc-1g8cvhx-0 jzJcTI">Ecommerce Plugins</p>
									</div>
								</div>
								<div class="Box-sc-5vx4ls-0 hAURWq">
									<h1
										class="Heading__StyledHeading-sc-10oikoy-0 kZQjgd ContentPageHeading__StyledHeading-sc-1ojl0u5-0 bRpweO">
										About Ecommerce Plugins</h1>
									<p class="Text-sc-1g8cvhx-0 gqQyhM">Check the list of Razorpay Ecommerce Plugins to
										integrate with the plugin of your choice and accept payments from your
										customers.</p>
									<hr class="Divider__StyledDivider-sc-5tlrkc-0 fONQLM" />
								</div>
								<main class="styled__ContentContainer-sc-fg4p2w-0 dPWSDH">
									<p class="Text-sc-1g8cvhx-0 Text__StyledTextComponent-sc-16y34hf-0 fhcimu eEHZvo">
										Integrate seamlessly with ecommerce platforms through our robust and secure
										plugins. You can accept payments via a range of payment methods like debit card,
										credit card, netbanking (supports 3D Secure), UPI and so on.</p>
									<article>
										<section>
											<h1 id="list-of-ecommerce-plugins"
												class="Heading__StyledHeading-sc-10oikoy-0 RtGqJ">
												<div display="flex"
													class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 dPVYbu fCPAWO Link__StyledLink-sc-38tiy-0 kWnpZi styled__StyledLink-sc-c6l8fk-0">
													<a target="_self"
														href="/docs/payments/payment-gateway/ecommerce-plugins#list-of-ecommerce-plugins">
														<p
															class="Text-sc-1g8cvhx-0 styled__StyledHeadingText-sc-c6l8fk-1 bNBVOX ggcwSt">
															List of Ecommerce Plugins</p><svg width="24" height="24"
															viewBox="0 0 24 24" fill="none"
															xmlns="http://www.w3.org/2000/svg"
															class="styled__StyledHeadingIcon-sc-c6l8fk-2 jITCZt">
															<path
																d="M21.1863 2.82377C18.8719 0.509364 15.1296 0.476845 12.7753 2.75068L12.765 2.7608L11.045 4.4708C10.6534 4.86019 10.6515 5.49335 11.0409 5.88501C11.4303 6.27667 12.0634 6.27852 12.4551 5.88913L14.1697 4.18451C15.7395 2.67341 18.2307 2.69666 19.772 4.23798C21.313 5.77898 21.3366 8.26948 19.8265 9.83934L16.833 12.8329C16.0124 13.6537 14.8758 14.0778 13.7181 13.9949C12.5605 13.9119 11.496 13.3303 10.8008 12.401C10.47 11.9587 9.84333 11.8684 9.40108 12.1992C8.95883 12.53 8.86849 13.1567 9.1993 13.5989C10.242 14.993 11.8388 15.8654 13.5753 15.9897C15.3117 16.1141 17.0165 15.4782 18.2473 14.2469L21.2472 11.2471L21.2593 11.2347C23.5332 8.8804 23.5007 5.13817 21.1863 2.82377Z"
																fill="#132644"></path>
															<path
																d="M10.4247 8.01016C8.68837 7.8858 6.9836 8.52171 5.75285 9.75283L2.75285 12.7528L2.74067 12.7652C0.466835 15.1195 0.499354 18.8617 2.81376 21.1761C5.12816 23.4905 8.8704 23.5231 11.2247 21.2492L11.2371 21.237L12.9471 19.527C13.3376 19.1365 13.3376 18.5034 12.9471 18.1128C12.5565 17.7223 11.9234 17.7223 11.5329 18.1128L9.82933 19.8164C8.25947 21.3265 5.76897 21.3029 4.22797 19.7619C2.68697 18.2209 2.66341 15.7304 4.17354 14.1606L7.16719 11.1669C7.9877 10.3461 9.12425 9.92214 10.2819 10.005C11.4395 10.088 12.504 10.6696 13.1992 11.5989C13.53 12.0412 14.1567 12.1315 14.5989 11.8007C15.0412 11.4699 15.1315 10.8432 14.8007 10.401C13.758 9.00693 12.1612 8.13452 10.4247 8.01016Z"
																fill="#132644"></path>
														</svg>
													</a></div>
											</h1>
											<p
												class="Text-sc-1g8cvhx-0 Text__StyledTextComponent-sc-16y34hf-0 fhcimu eEHZvo">
												Razorpay offers a list of ecommerce plugins given below:</p>
											<ul class="styled__StyledUl-sc-hqnxju-1 gcqLlE">
												<li class="styled__StyledLi-sc-hqnxju-2 jszEzM">
													<div display="inline-flex"
														class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 lpjypG fCPAWO Link__StyledLink-sc-38tiy-0 kWnpZi styled__StyledContentLink-sc-r9g6hi-0 chZHUd">
														<a target="_blank"
															href="/docs/payments/payment-gateway/ecommerce-plugins/arastta">
															<p
																class="Text-sc-1g8cvhx-0 Link__StyledText-sc-38tiy-2 dePkrl fLetpi">
																Arastta</p>
														</a></div>
												</li>
												<li class="styled__StyledLi-sc-hqnxju-2 jszEzM">
													<div display="inline-flex"
														class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 lpjypG fCPAWO Link__StyledLink-sc-38tiy-0 kWnpZi styled__StyledContentLink-sc-r9g6hi-0 chZHUd">
														<a target="_blank"
															href="/docs/payments/payment-gateway/ecommerce-plugins/bigcommerce">
															<p
																class="Text-sc-1g8cvhx-0 Link__StyledText-sc-38tiy-2 dePkrl fLetpi">
																BigCommerce</p>
														</a></div>
												</li>
												<li class="styled__StyledLi-sc-hqnxju-2 jszEzM">
													<div display="inline-flex"
														class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 lpjypG fCPAWO Link__StyledLink-sc-38tiy-0 kWnpZi styled__StyledContentLink-sc-r9g6hi-0 chZHUd">
														<a target="_blank"
															href="/docs/payments/payment-gateway/ecommerce-plugins/cs-cart">
															<p
																class="Text-sc-1g8cvhx-0 Link__StyledText-sc-38tiy-2 dePkrl fLetpi">
																CS-Cart</p>
														</a></div>
												</li>
												<li class="styled__StyledLi-sc-hqnxju-2 jszEzM">
													<div display="inline-flex"
														class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 lpjypG fCPAWO Link__StyledLink-sc-38tiy-0 kWnpZi styled__StyledContentLink-sc-r9g6hi-0 chZHUd">
														<a target="_blank"
															href="/docs/payments/payment-gateway/ecommerce-plugins/drupal-commerce">
															<p
																class="Text-sc-1g8cvhx-0 Link__StyledText-sc-38tiy-2 dePkrl fLetpi">
																Drupal Commerce</p>
														</a></div>
												</li>
												<li class="styled__StyledLi-sc-hqnxju-2 jszEzM">
													<div display="inline-flex"
														class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 lpjypG fCPAWO Link__StyledLink-sc-38tiy-0 kWnpZi styled__StyledContentLink-sc-r9g6hi-0 chZHUd">
														<a target="_blank"
															href="/docs/payments/payment-gateway/ecommerce-plugins/easy-digital-downloads">
															<p
																class="Text-sc-1g8cvhx-0 Link__StyledText-sc-38tiy-2 dePkrl fLetpi">
																Easy Digital Downloads</p>
														</a></div>
												</li>
												<li class="styled__StyledLi-sc-hqnxju-2 jszEzM">
													<div display="inline-flex"
														class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 lpjypG fCPAWO Link__StyledLink-sc-38tiy-0 kWnpZi styled__StyledContentLink-sc-r9g6hi-0 chZHUd">
														<a target="_blank"
															href="/docs/payments/payment-gateway/ecommerce-plugins/gravity-forms">
															<p
																class="Text-sc-1g8cvhx-0 Link__StyledText-sc-38tiy-2 dePkrl fLetpi">
																Gravity Forms</p>
														</a></div>
												</li>
												<li class="styled__StyledLi-sc-hqnxju-2 jszEzM">
													<div display="inline-flex"
														class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 lpjypG fCPAWO Link__StyledLink-sc-38tiy-0 kWnpZi styled__StyledContentLink-sc-r9g6hi-0 chZHUd">
														<a target="_blank"
															href="/docs/payments/payment-gateway/ecommerce-plugins/magento">
															<p
																class="Text-sc-1g8cvhx-0 Link__StyledText-sc-38tiy-2 dePkrl fLetpi">
																Magento</p>
														</a></div>
												</li>
												<li class="styled__StyledLi-sc-hqnxju-2 jszEzM">
													<div display="inline-flex"
														class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 lpjypG fCPAWO Link__StyledLink-sc-38tiy-0 kWnpZi styled__StyledContentLink-sc-r9g6hi-0 chZHUd">
														<a target="_blank"
															href="/docs/payments/payment-gateway/ecommerce-plugins/open-cart">
															<p
																class="Text-sc-1g8cvhx-0 Link__StyledText-sc-38tiy-2 dePkrl fLetpi">
																OpenCart</p>
														</a></div>
												</li>
												<li class="styled__StyledLi-sc-hqnxju-2 jszEzM">
													<div display="inline-flex"
														class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 lpjypG fCPAWO Link__StyledLink-sc-38tiy-0 kWnpZi styled__StyledContentLink-sc-r9g6hi-0 chZHUd">
														<a target="_blank"
															href="/docs/payments/payment-gateway/ecommerce-plugins/prestashop">
															<p
																class="Text-sc-1g8cvhx-0 Link__StyledText-sc-38tiy-2 dePkrl fLetpi">
																PrestaShop</p>
														</a></div>
												</li>
												<li class="styled__StyledLi-sc-hqnxju-2 jszEzM">
													<div display="inline-flex"
														class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 lpjypG fCPAWO Link__StyledLink-sc-38tiy-0 kWnpZi styled__StyledContentLink-sc-r9g6hi-0 chZHUd">
														<a target="_blank"
															href="/docs/payments/payment-gateway/ecommerce-plugins/shopify">
															<p
																class="Text-sc-1g8cvhx-0 Link__StyledText-sc-38tiy-2 dePkrl fLetpi">
																Shopify</p>
														</a></div>
												</li>
												<li class="styled__StyledLi-sc-hqnxju-2 jszEzM">
													<div display="inline-flex"
														class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 lpjypG fCPAWO Link__StyledLink-sc-38tiy-0 kWnpZi styled__StyledContentLink-sc-r9g6hi-0 chZHUd">
														<a target="_blank"
															href="/docs/payments/payment-gateway/ecommerce-plugins/whmcs">
															<p
																class="Text-sc-1g8cvhx-0 Link__StyledText-sc-38tiy-2 dePkrl fLetpi">
																WHMCS</p>
														</a></div>
												</li>
												<li class="styled__StyledLi-sc-hqnxju-2 jszEzM">
													<div display="inline-flex"
														class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 lpjypG fCPAWO Link__StyledLink-sc-38tiy-0 kWnpZi styled__StyledContentLink-sc-r9g6hi-0 chZHUd">
														<a target="_blank"
															href="/docs/payments/payment-gateway/ecommerce-plugins/wix">
															<p
																class="Text-sc-1g8cvhx-0 Link__StyledText-sc-38tiy-2 dePkrl fLetpi">
																Wix</p>
														</a></div>
												</li>
												<li class="styled__StyledLi-sc-hqnxju-2 jszEzM">
													<div display="inline-flex"
														class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 lpjypG fCPAWO Link__StyledLink-sc-38tiy-0 kWnpZi styled__StyledContentLink-sc-r9g6hi-0 chZHUd">
														<a target="_blank"
															href="/docs/payments/payment-gateway/ecommerce-plugins/woocommerce">
															<p
																class="Text-sc-1g8cvhx-0 Link__StyledText-sc-38tiy-2 dePkrl fLetpi">
																WooCommerce</p>
														</a></div>
												</li>
												<li class="styled__StyledLi-sc-hqnxju-2 jszEzM">
													<div display="inline-flex"
														class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 lpjypG fCPAWO Link__StyledLink-sc-38tiy-0 kWnpZi styled__StyledContentLink-sc-r9g6hi-0 chZHUd">
														<a target="_blank"
															href="/docs/payments/payment-gateway/ecommerce-plugins/wordpress">
															<p
																class="Text-sc-1g8cvhx-0 Link__StyledText-sc-38tiy-2 dePkrl fLetpi">
																WordPress</p>
														</a></div>
												</li>
											</ul>
											<p
												class="Text-sc-1g8cvhx-0 Text__StyledTextComponent-sc-16y34hf-0 fhcimu eEHZvo">
												You can <div display="inline-flex"
													class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 lpjypG fCPAWO Link__StyledLink-sc-38tiy-0 kWnpZi styled__StyledContentLink-sc-r9g6hi-0 chZHUd">
													<a target="_blank"
														href="/docs/payments/payment-gateway/ecommerce-plugins/build-your-own">
														<p
															class="Text-sc-1g8cvhx-0 Link__StyledText-sc-38tiy-2 dePkrl fLetpi">
															build your own plugin</p>
													</a></div> in case the plugin you are looking for is not listed
												above.</p>
										</section>
									</article>
									<article>
										<section>
											<h1 id="related-information"
												class="Heading__StyledHeading-sc-10oikoy-0 RtGqJ">
												<div display="flex"
													class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 dPVYbu fCPAWO Link__StyledLink-sc-38tiy-0 kWnpZi styled__StyledLink-sc-c6l8fk-0">
													<a target="_self"
														href="/docs/payments/payment-gateway/ecommerce-plugins#related-information">
														<p
															class="Text-sc-1g8cvhx-0 styled__StyledHeadingText-sc-c6l8fk-1 bNBVOX ggcwSt">
															Related Information</p><svg width="24" height="24"
															viewBox="0 0 24 24" fill="none"
															xmlns="http://www.w3.org/2000/svg"
															class="styled__StyledHeadingIcon-sc-c6l8fk-2 jITCZt">
															<path
																d="M21.1863 2.82377C18.8719 0.509364 15.1296 0.476845 12.7753 2.75068L12.765 2.7608L11.045 4.4708C10.6534 4.86019 10.6515 5.49335 11.0409 5.88501C11.4303 6.27667 12.0634 6.27852 12.4551 5.88913L14.1697 4.18451C15.7395 2.67341 18.2307 2.69666 19.772 4.23798C21.313 5.77898 21.3366 8.26948 19.8265 9.83934L16.833 12.8329C16.0124 13.6537 14.8758 14.0778 13.7181 13.9949C12.5605 13.9119 11.496 13.3303 10.8008 12.401C10.47 11.9587 9.84333 11.8684 9.40108 12.1992C8.95883 12.53 8.86849 13.1567 9.1993 13.5989C10.242 14.993 11.8388 15.8654 13.5753 15.9897C15.3117 16.1141 17.0165 15.4782 18.2473 14.2469L21.2472 11.2471L21.2593 11.2347C23.5332 8.8804 23.5007 5.13817 21.1863 2.82377Z"
																fill="#132644"></path>
															<path
																d="M10.4247 8.01016C8.68837 7.8858 6.9836 8.52171 5.75285 9.75283L2.75285 12.7528L2.74067 12.7652C0.466835 15.1195 0.499354 18.8617 2.81376 21.1761C5.12816 23.4905 8.8704 23.5231 11.2247 21.2492L11.2371 21.237L12.9471 19.527C13.3376 19.1365 13.3376 18.5034 12.9471 18.1128C12.5565 17.7223 11.9234 17.7223 11.5329 18.1128L9.82933 19.8164C8.25947 21.3265 5.76897 21.3029 4.22797 19.7619C2.68697 18.2209 2.66341 15.7304 4.17354 14.1606L7.16719 11.1669C7.9877 10.3461 9.12425 9.92214 10.2819 10.005C11.4395 10.088 12.504 10.6696 13.1992 11.5989C13.53 12.0412 14.1567 12.1315 14.5989 11.8007C15.0412 11.4699 15.1315 10.8432 14.8007 10.401C13.758 9.00693 12.1612 8.13452 10.4247 8.01016Z"
																fill="#132644"></path>
														</svg>
													</a></div>
											</h1>
											<ul class="styled__StyledUl-sc-hqnxju-1 gcqLlE">
												<li class="styled__StyledLi-sc-hqnxju-2 jszEzM">
													<div display="inline-flex"
														class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 lpjypG fCPAWO Link__StyledLink-sc-38tiy-0 kWnpZi styled__StyledContentLink-sc-r9g6hi-0 chZHUd">
														<a target="_blank"
															href="/docs/payments/payment-gateway/how-it-works">
															<p
																class="Text-sc-1g8cvhx-0 Link__StyledText-sc-38tiy-2 dePkrl fLetpi">
																How Payment Gateway Works</p>
														</a></div>
												</li>
												<li class="styled__StyledLi-sc-hqnxju-2 jszEzM">
													<div display="inline-flex"
														class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 lpjypG fCPAWO Link__StyledLink-sc-38tiy-0 kWnpZi styled__StyledContentLink-sc-r9g6hi-0 chZHUd">
														<a target="_blank"
															href="/docs/payments/payment-gateway/features/">
															<p
																class="Text-sc-1g8cvhx-0 Link__StyledText-sc-38tiy-2 dePkrl fLetpi">
																Features</p>
														</a></div>
												</li>
												<li class="styled__StyledLi-sc-hqnxju-2 jszEzM">
													<div display="inline-flex"
														class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 lpjypG fCPAWO Link__StyledLink-sc-38tiy-0 kWnpZi styled__StyledContentLink-sc-r9g6hi-0 chZHUd">
														<a target="_blank"
															href="/docs/payments/payment-methods#supported-payment-methods">
															<p
																class="Text-sc-1g8cvhx-0 Link__StyledText-sc-38tiy-2 dePkrl fLetpi">
																Supported Payment Methods</p>
														</a></div>
												</li>
											</ul>
										</section>
									</article>
								</main>
							</div>
							<div data-blade-component="box" class="BaseBoxweb__BaseBox-sc-1icfu8j-0">
								<hr class="Divider__StyledDivider-sc-5tlrkc-0 fONQLM" />
								<div data-blade-component="box" class="BaseBoxweb__BaseBox-sc-1icfu8j-0 hNwRVL">
									<div display="flex"
										class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 dPVYbu foqTwv">
										<p class="Text-sc-1g8cvhx-0 ikQWpa">Was this page helpful?</p>
										<div display="flex"
											class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 dPVYbu eFTsHp">
											<button class="Button__StyledButton-sc-1g40twz-0 rDRVp styles__PositiveFeedbackButton-sc-1ahuhrc-0 emxFrX"><p class="Text-sc-1g8cvhx-0 Button__StyledText-sc-1g40twz-1 HSevc imbcFy">Yes</p></button><button class="Button__StyledButton-sc-1g40twz-0 rDRVp styles__NegativeFeedbackButton-sc-1ahuhrc-1 etjtqK"><p class="Text-sc-1g8cvhx-0 Button__StyledText-sc-1g40twz-1 HSevc imbcFy">No</p></button>
										</div>
									</div>
								</div>
							</div>
							<footer class="Box-sc-5vx4ls-0 cGOgLs">
								<hr class="Divider__StyledDivider-sc-5tlrkc-0 fONQLM" />
								<p class="Text-sc-1g8cvhx-0 ckbwmr">SUBSCRIBE TO DEVELOPER UPDATES</p>
								<div display="flex" class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 dPVYbu knXDpV">
									<div display="flex"
										class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 kHUkaB gyXFoV">
										<div display="flex" width="100%" type="email" name="email" required=""
											aria-label="Your email address"
											class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 dcjpbN jcarLi Input__StyledInputContainer-sc-1p8iijo-3 iZtQst DeveloperSubscription__StyledSubscriptionInput-sc-1gbefub-0 fTHyQm">
											<input type="email" placeholder="Your email address" value="" name="email" required="" aria-label="Your email address" class="Input__StyledInput-sc-1p8iijo-2 bxdbSG DeveloperSubscription__StyledSubscriptionInput-sc-1gbefub-0 fTHyQm"/><button class="Button__StyledButton-sc-1g40twz-0 fNlFXx Input__StyledButtonRight-sc-1p8iijo-1"><p class="Text-sc-1g8cvhx-0 Button__StyledText-sc-1g40twz-1 IPzaW imbcFy">Subscribe</p></button>
										</div>
										<p color="hsla(8, 73%, 47%, 1)"
											class="Text-sc-1g8cvhx-0 DeveloperSubscription__StyledErrorText-sc-1gbefub-1 dWSCQs iAimGP">
										</p>
									</div>
									<div display="flex"
										class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 dPVYbu jKPpuE Footer__FooterLinkContainer-sc-1snnb4l-0 etdARH">
										<div display="flex"
											class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 dPVYbu fCPAWO Link__StyledLink-sc-38tiy-0 kWnpZi">
											<a target="_self" href="/docs/api">
												<p class="Text-sc-1g8cvhx-0 Link__StyledText-sc-38tiy-2 bjKbMn fLetpi">
													API Reference Guide</p>
											</a></div>
										<div display="flex"
											class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 dPVYbu fCPAWO Link__StyledLink-sc-38tiy-0 kWnpZi">
											<a href="https://razorpay.com/integrations" target="_self"
												rel="noopener noreferrer">
												<p class="Text-sc-1g8cvhx-0 Link__StyledText-sc-38tiy-2 bjKbMn fLetpi">
													Integrations</p>
											</a></div>
										<div display="flex"
											class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 dPVYbu fCPAWO Link__StyledLink-sc-38tiy-0 kWnpZi">
											<a href="https://razorpay.com/support" target="_self"
												rel="noopener noreferrer">
												<p class="Text-sc-1g8cvhx-0 Link__StyledText-sc-38tiy-2 bjKbMn fLetpi">
													Support</p>
											</a></div>
									</div>
								</div>
							</footer>
						</div>
						<div display="[object Object]" width="240" height="calc(100vh - 68px)"
							class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 igNNgb tGMIa">
							<div overflow="hidden" class="Box-sc-5vx4ls-0 foKBkC">
								<div display="flex" height="100%"
									class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 llIhct gyXFoV">
									<p class="Text-sc-1g8cvhx-0 erLHrN">ON THIS PAGE</p>
									<ul class="TableOfContents__ContentListContainer-sc-g0fs5p-0 hZUQuc">
										<li data-active="li-state-active-true"
											class="Box-sc-5vx4ls-0 TableOfContents__ContentListItem-sc-g0fs5p-1 eaPebU gGzofQ">
											<div display="flex"
												class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 dPVYbu fCPAWO Link__StyledLink-sc-38tiy-0 kWnpZi">
												<a target="_self"
													href="/docs/payments/payment-gateway/ecommerce-plugins#list-of-ecommerce-plugins">
													<p
														class="Text-sc-1g8cvhx-0 Link__StyledText-sc-38tiy-2 iKTxur fLetpi">
														List of Ecommerce Plugins</p>
												</a></div>
										</li>
										<li data-active="li-state-active-false"
											class="Box-sc-5vx4ls-0 TableOfContents__ContentListItem-sc-g0fs5p-1 eaPebU ebOfVV">
											<div display="flex"
												class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 dPVYbu fCPAWO Link__StyledLink-sc-38tiy-0 kWnpZi">
												<a target="_self"
													href="/docs/payments/payment-gateway/ecommerce-plugins#related-information">
													<p
														class="Text-sc-1g8cvhx-0 Link__StyledText-sc-38tiy-2 iKTxur kkMCYI">
														Related Information</p>
												</a></div>
										</li>
									</ul>
								</div>
							</div>
							<div display="flex" class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 dPVYbu tGMIa">
								<div display="flex" class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 hUQOpC gbpuuV">
								</div>
							</div>
						</div>
						<button id="scroll-top-button" width="fit-content" class="Box-sc-5vx4ls-0 ScrollTop__StyledScrollTop-sc-1qkh247-0 iKxIPs ircWIJ"><div display="flex" class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 iXFBBH hDYGnW"><div display="flex" width="[object Object]" height="[object Object]" class="Box-sc-5vx4ls-0 Flex__StyledFlex-sc-1n8gmmd-0 kkSa-dm fxAeXL ScrollTop__StyledUpArrow-sc-1qkh247-1 gcQOFV"><svg width="20" height="20" viewBox="0 0 24 24" fill="none"><path d="M12.707 3.293a1 1 0 0 0-1.414 0l-6 6a1 1 0 0 0 1.414 1.414L11 6.414V20a1 1 0 1 0 2 0V6.414l4.293 4.293a1 1 0 0 0 1.414-1.414l-6-6Z" fill="hsla(216, 16%, 60%, 1)"></path></svg></div></div></button>
					</div>
				</div>
			</div>
		</div>
	</div>
	<script id="__LOADABLE_REQUIRED_CHUNKS__" type="application/json">
		[]
	</script>
	<script id="__LOADABLE_REQUIRED_CHUNKS___ext" type="application/json">
		{"namedChunks":[]}
	</script>
	<script async="" data-chunk="main" src="/docs/build/browser/js/runtime.a17d3a71.js"></script>
	<script async="" data-chunk="main" src="/docs/build/browser/js/51513.dedbf6a9.js"></script>
	<script async="" data-chunk="main" src="/docs/build/browser/js/23825.0c60d07a.js"></script>
	<script async="" data-chunk="main" src="/docs/build/browser/js/main.d0c7b243.js"></script>
	<script defer="" data-chunk="client" src="/docs/build/browser/js/98445.b4190deb.js"></script>
	<script defer="" data-chunk="client" src="/docs/build/browser/js/client.25de0159.js"></script>
</body>

</html>

```

- What status code did you get back?

> 200

- Click on the **response** headers in Postman. What are the `Content-Type` and `Content-Length` (provide exact values)?

> `Content-Type` text/html

> `Content-Length` 

- Summarize the most salient parts of the data you are getting back (for example, Cat facts returns JSON that identifies the source of the cat fact, the cat fact, information about when the fact was created and updated, and the fact itself).

> The summary of the data is ...

- How could you use this data in an application?

> I could imagine integrating this API into an app that handles payroll, or is used to place autopayment tools/reminders

- What did you like about the documentation?

> The documentation was simple to understnad and not too wordy

- What did you find challenging about the documentation?

> I found the documentation it was a little hard to find the about section

- Did the quality of the documentation impact your decision to use it?

> Yes because too much documentation can make it hard to keep interted in what the API has to offer.

- Did you switch which API you chose initially because of its documentation, or did you stick with the one you selected and work your way through it?

> no changed my API because the website carshed for one and the other is going out of business.

- In your own words, summarize the request-response cycle.

> The request-response cycle a process in which a user and a serve communicate to render a webpage and its functions

- In your own words, describe what an API is.

> An API is a tool used to get apps and tools to work together

- In your own words, describe the purpose of Postman.

> Postman is an application that helps programers work and develop thier API
