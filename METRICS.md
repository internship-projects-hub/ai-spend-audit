# METRICS.md

## North Star Metric
Number of completed audits with email capture

Reason:
This directly reflects both user value (audit completed) and business value (lead generation for Credex).

---

## Input Metrics

1. Landing page visitors
2. Form completion rate (input → audit start)
3. Audit completion rate
4. Email capture rate

---

## Instrumentation Plan

Track:
- page_view
- form_start
- form_submit
- audit_complete
- email_submit

Using simple analytics (or Supabase events table)

---

## Pivot Trigger

If:
- audit completion rate < 40%
OR
- email capture rate < 10%

Then:
→ UX or value proposition needs redesign

---

## Summary
The product is successful only if users complete audits and leave emails, not just visit the page.