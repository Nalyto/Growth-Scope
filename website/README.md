# GrowthScope Website

Marketing website for GrowthScope, isolated from the existing app.

## Preview URL
After GitHub Pages publishes the commit, visit:
https://syh18.github.io/Growth-Scope/website/

## Safety
- The existing root `index.html` application is unchanged.
- No Supabase tables, policies, authentication settings, or user data are changed.
- All "Login", "Mulai Gratis", and "Buka GrowthScope" links currently route to the existing app:
  https://syh18.github.io/Growth-Scope/
- The paid-plan modal is an interest-form prototype only. It downloads a JSON summary in the visitor's browser; it does not send a lead to GrowthScope and does not charge or create a subscription.

## Before accepting paid subscriptions
1. Choose a payment provider that supports your business and target market (for example, Midtrans or Xendit in Indonesia, subject to account approval).
2. Implement a trusted server-side checkout/session endpoint and payment webhooks. Do not put secret keys in this static site.
3. Add subscription records and server-side plan/entitlement checks to the existing Supabase architecture without deleting or recreating existing tables.
4. Define plan limits, billing cycle, taxes/refunds, cancellation, and customer support terms.
5. Connect a real lead/contact endpoint and add privacy policy, terms, and support contact details.
6. Test signup, checkout, failed payments, renewal, cancellation, and access revocation with test credentials before production.

## Pricing displayed
Business: Rp399.000/month
Agency: Rp999.000/month
The annual view shows an estimated 15% discount equivalent per month. These are draft pricing concepts, not active purchasable offers. Review limits and actual included features before enabling checkout.
