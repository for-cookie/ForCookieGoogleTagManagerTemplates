# ForCookie Consent Management (GTM Template)

ForCookie is a lightweight consent management solution designed to integrate with Google Tag Manager (GTM) and Google Consent Mode v2.

It allows website owners to collect and manage user cookie preferences and control GTM tags based on user consent.

---

## 🚀 Features

- Google Consent Mode v2 support
- GTM native template integration
- Control over analytics and marketing tags
- GDPR / KVKK / LGPD compliant consent flow
- Lightweight and fast execution
- No external tracking of user consent data

---

## 📦 Installation (Google Tag Manager)

1. Open your Google Tag Manager account
2. Go to **Templates → Tag Templates**
3. Click **Search Gallery**
4. Import the ForCookie template
5. Create a new tag using the template
6. Set trigger to:

   **Consent Initialization – All Pages**
7. Publish your container

---

## ⚙️ How it works

ForCookie works with Google Consent Mode by setting default consent states on page load and updating them based on user interaction.

### Default state (on page load)

- analytics_storage: denied
- ad_storage: denied
- functionality_storage: denied

### User interaction

When a user updates their preferences, consent states are updated via GTM Consent API.

---

## 🔄 Consent Flow

Page Load  
→ Default consent is set (denied)

User selects preferences  
→ Consent is updated via GTM

GTM Tags  
→ Execute based on consent state

---

## 🌐 Data Privacy

ForCookie does not collect, store, or transmit any personal user data outside of the website where it is installed.

No consent or tracking data is sent to external servers.

The only external domain used is:

- https://www.forcookie.com (documentation and support only)

---

## 🧩 GTM Integration

This template is designed for use inside Google Tag Manager only.

All tracking tags (GA4, Ads, etc.) must be managed through GTM and respect Consent Mode settings.

---

## 📌 Requirements

- Google Tag Manager container
- Consent Mode v2 enabled
- All marketing tags configured inside GTM

---

## 🔐 Compliance

This template is designed to help comply with:

- GDPR
- ePrivacy Directive
- KVKK
- LGPD

However, legal compliance depends on your implementation.

---

## 📖 Versioning

All template versions are tracked via Git commit SHA in metadata.yaml.

---

## 🧠 Important Notes

- This template does not automatically block GTM
- It only controls consent signals inside GTM
- Incorrect GTM setup may result in tracking misconfiguration

---

## 📞 Support & Documentation

For detailed installation and setup guides:

- **Turkish (TR):** https://www.forcookie.com/forcookie-tagmanager-nasil-kurulur/
- **English (EN):** https://www.forcookie.com/en/forcookie-install-tagmanager/

General support: https://www.forcookie.com
