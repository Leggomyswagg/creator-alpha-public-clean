# CreatorAlpha static prototype

The repository contains a self-contained compiled React app in `index.html`, served as a static site. `npm run build` completes the static build; Vercel uses the included `vercel.json`.

## Available behavior

- The ranking starts empty; entering a domain generates two local example idea templates.
- Profiles, saved ideas, categories, and checklist progress persist in this browser's local storage.
- Saved playbook checkboxes update immediately in both the open playbook and vault. Completion updates the idea's status.
- The iOS deployment button is removed from this public build.

## Work required before a production service

The domain generator does not fetch or analyze a website. Its opportunity scores and revenue projections are simulated examples, not measured market data. Real scanning needs a backend and a defined source of evidence.

The profile, plan, pricing, and founder-code controls are browser-only demonstrations. There is no authentication, subscription verification, or payment integration. Public client configuration cannot serve as a secret or enforce paid access; Vercel environment variables are not substituted into this precompiled static HTML. Add server-side authentication and entitlements before using these controls for a paid product.

Editable component sources and the original build configuration are absent. Restore them before making broader product changes. Clearing browser data resets local saved work; there is no account synchronization.
