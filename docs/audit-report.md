# Accessibility Audit Report

## 1. Audited Website

**Website:** Tamil Nadu e-Sevai Citizen Portal

**Page Audited:** Citizen Portal Login

## 2. Audit Methods

The website was evaluated using:

- Google Chrome Lighthouse Accessibility audit
- Manual keyboard-only navigation
- Tab and Shift + Tab navigation testing

## 3. Lighthouse Result

**Accessibility Score:** 70

## 4. Findings

### Issue 1 — Insufficient Color Contrast

**Category:** Contrast

**Finding:** Background and foreground colors do not have a sufficient contrast ratio.

**Evidence:** Lighthouse Accessibility audit.

**Impact:** Low-contrast content can be difficult for some users to read.

**Suggested Remediation:** Adjust foreground and background colors to provide sufficient contrast.

**Evidence:** `lighthouse-01-contrast.png`

---

### Issue 2 — Positive Tabindex Values

**Category:** Navigation

**Finding:** Some elements have a tabindex value greater than 0.

**Evidence:** Lighthouse identified username, password, CAPTCHA and login elements.

**Impact:** Positive tabindex values can create an unexpected keyboard navigation order.

**Suggested Remediation:** Avoid positive tabindex values and use the natural HTML focus order where possible.

**Evidence:** `lighthouse-02-tabindex.png`

---

### Issue 3 — Link Without a Discernible Name

**Category:** Names and Labels

**Finding:** A link does not have a discernible name.

**Evidence:** Lighthouse identified a link element without a discernible accessible name.

**Impact:** Screen-reader users may have difficulty understanding the purpose of the link.

**Suggested Remediation:** Provide meaningful link text or an appropriate accessible name.

**Evidence:** `lighthouse-03-link-name.png`

---

### Issue 4 — Missing HTML Language Attribute

**Category:** Internationalization and Localization

**Finding:** The HTML element does not have a lang attribute.

**Evidence:** Lighthouse identified the HTML element as missing a lang attribute.

**Impact:** Screen readers may not correctly determine the language of the page, which can affect pronunciation.

**Suggested Remediation:** Add an appropriate lang attribute to the HTML element.

**Evidence:** `lighthouse-05-lang-attribute.png`

---

### Issue 5 — Insufficient Touch Target Size or Spacing

**Category:** Best Practices

**Finding:** Touch targets do not have sufficient size or spacing.

**Evidence:** Lighthouse identified multiple link elements as insufficiently sized or spaced touch targets.

**Impact:** Small or closely spaced controls can be difficult to activate, particularly on touch devices.

**Suggested Remediation:** Increase interactive target sizes and provide sufficient spacing between adjacent controls.

**Evidence:** `lighthouse-04-touch-targets.png`

---

## 5. Keyboard-Only Navigation Pass

A manual keyboard-only navigation test was performed using the Tab and Shift + Tab keys.

The Tab key moved through the interactive elements sequentially, including navigation items such as Home and About Us. Shift + Tab successfully moved backward through the elements.

No keyboard trap was observed during the test.

### Result

The keyboard-only navigation test was completed successfully, and no additional keyboard-navigation issue was identified during the manual test.
