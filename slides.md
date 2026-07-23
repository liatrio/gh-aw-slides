---
theme: slidev-theme-liatrio
title: Slidev Theme Liatrio — Test Deck
mdc: true
layout: cover-with-image
image: /liatris-single.png
backgroundSize: contain
---

<div class="eyebrow">Liatrio · Slidev theme</div>

# Testing the <span class="accent">Liatrio theme.</span>

### A sample deck built from the local theme package

<!--
f
-->

---
layout: agenda
---

<div class="eyebrow">On the docket</div>

# What this deck <span class="accent">covers.</span>

1. **Chapters & sections** How the theme breaks up a narrative.
2. **Layouts** Two-column, image, and stats layouts in action.
3. **Components** Portraits, capability icons, and QR codes.
4. **Code & quotes** Syntax highlighting and pull quotes.

---
layout: chapter
---

<div class="eyebrow">Section one</div>

# Layouts <span class="accent">tour.</span>

---
layout: two-cols
---

<div class="eyebrow">Structure</div>

### Content on the left

Two-column layouts split the canvas evenly. Lead with the narrative here, then support it with detail on the other side.

::right::

<div class="eyebrow">Detail</div>

### Detail on the right

The `::right::` marker sends everything after it into the second column.

---
layout: image-right
image: /venn-pillars.png
backgroundSize: contain
---

<div class="eyebrow">How it fits together</div>

# Three pillars, one <span class="accent">practice.</span>

<hr class="rule" />

- People, process, and technology in balance
- Delivered as a continuous engineering practice
- Measured against outcomes, not output

---
layout: stats
---

<div class="eyebrow">By the numbers</div>

# A few made-up <span class="accent">metrics.</span>

<div class="stats-grid">
  <div class="card">
    <div class="stat-label">Deploy frequency</div>
    <div class="stat-num">14x</div>
    <p>More frequent releases after adopting a platform engineering model.</p>
  </div>
  <div class="card">
    <div class="stat-label">Lead time</div>
    <div class="stat-num">60%</div>
    <p>Reduction in time from commit to production across pilot teams.</p>
  </div>
  <div class="card">
    <div class="stat-label">Adoption</div>
    <div class="stat-num">90%</div>
    <p>Of engineers active on the internal developer platform within a quarter.</p>
  </div>
</div>

---
layout: chapter
---

<div class="eyebrow">Section two</div>

# Components <span class="accent">tour.</span>

---
layout: default
---

<div class="eyebrow">Meet the team</div>

# A face to the <span class="accent">work.</span>

<hr class="rule" />

<Portrait src="/avatar.png" name="Ada Lovelace" title="Principal Engineer" desc="Writes the first program, reviews the last PR." email="ada@example.com" />

---
layout: default
---

<div class="eyebrow">What we do</div>

# Capabilities at a <span class="accent">glance.</span>

<hr class="rule" />

<div class="grid grid-cols-3 gap-4">
  <Icon icon="security" />
  <Icon icon="cloud-native" />
  <Icon icon="enablement" />
  <Icon icon="platforms" />
  <Icon icon="mlops" />
  <Icon icon="modernization" />
</div>

---
layout: default
---

<div class="eyebrow">Live highlighting</div>

# Code, rendered in <span class="accent">context.</span>

<hr class="rule" />

```ts
interface Deployment {
  service: string
  environment: 'staging' | 'production'
  version: string
}

async function promote(deploy: Deployment) {
  const gate = await checkPolicy(deploy)
  if (!gate.approved)
    throw new Error(`Blocked: ${gate.reason}`)
  return ship(deploy)
}
```

---
layout: default
---

<div class="eyebrow">Take it with you</div>

# Scan to learn <span class="accent">more.</span>

<hr class="rule" />

<div class="flex items-center gap-8">
  <QRCode value="https://liatrio.com" :size="180" />
  <div>
    Point a camera at the code to open <strong>liatrio.com</strong>. The component accepts <code>value</code>, <code>size</code>, <code>foreground</code>, and <code>background</code> props.
  </div>
</div>

---
layout: quote
---

Testing a theme locally is just <span class="accent">good practice.</span>

::eyebrow::

A note to self

::attribution::

Author of this deck

---
layout: about
---

<div class="eyebrow">Who we are</div>

# This is a <span class="accent">test deck.</span>

<hr class="rule" />

Built in `slidev-test` against the local copy of `slidev-theme-liatrio` to confirm layouts, components, and styling all resolve correctly before publishing the theme.

---
layout: mic-drop
---

Thank you<span class="accent">.</span>

::eyebrow::

End of test deck
