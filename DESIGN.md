---
version: alpha
name: AI Meeting Companion
description: Compact iOS meeting overview with violet AI accents, lightweight decisions, and grouped action items.
colors:
  primary: '#7540F5'
  primary-strong: '#6330D9'
  primary-soft: '#F2EDFF'
  neutral: '#FCFCFE'
  surface: '#FFFFFF'
  on-surface: '#11101A'
  secondary: '#646775'
  muted: '#707481'
  border: '#E4E5EB'
  control-outline: '#858996'
  priority-surface: '#FFE3DA'
  priority-text: '#9B311F'
  done-surface: '#F0F0F3'
  done-text: '#616472'
typography:
  headline-lg:
    fontFamily: -apple-system, BlinkMacSystemFont, "SF Pro Text", "Segoe UI", sans-serif
    fontSize: 28px
    fontWeight: 700
    lineHeight: 34px
  headline-md:
    fontFamily: -apple-system, BlinkMacSystemFont, "SF Pro Text", "Segoe UI", sans-serif
    fontSize: 20px
    fontWeight: 700
    lineHeight: 25px
  label-ai:
    fontFamily: -apple-system, BlinkMacSystemFont, "SF Pro Text", "Segoe UI", sans-serif
    fontSize: 17px
    fontWeight: 600
    lineHeight: 22px
  label-lg:
    fontFamily: -apple-system, BlinkMacSystemFont, "SF Pro Text", "Segoe UI", sans-serif
    fontSize: 16px
    fontWeight: 600
    lineHeight: 21px
  label-md:
    fontFamily: -apple-system, BlinkMacSystemFont, "SF Pro Text", "Segoe UI", sans-serif
    fontSize: 15px
    fontWeight: 600
    lineHeight: 20px
  body-lg:
    fontFamily: -apple-system, BlinkMacSystemFont, "SF Pro Text", "Segoe UI", sans-serif
    fontSize: 16px
    fontWeight: 400
    lineHeight: 22px
  body-md:
    fontFamily: -apple-system, BlinkMacSystemFont, "SF Pro Text", "Segoe UI", sans-serif
    fontSize: 15px
    fontWeight: 400
    lineHeight: 21px
  body-sm:
    fontFamily: -apple-system, BlinkMacSystemFont, "SF Pro Text", "Segoe UI", sans-serif
    fontSize: 14px
    fontWeight: 400
    lineHeight: 20px
  caption:
    fontFamily: -apple-system, BlinkMacSystemFont, "SF Pro Text", "Segoe UI", sans-serif
    fontSize: 13px
    fontWeight: 400
    lineHeight: 18px
  badge:
    fontFamily: -apple-system, BlinkMacSystemFont, "SF Pro Text", "Segoe UI", sans-serif
    fontSize: 12px
    fontWeight: 500
    lineHeight: 16px
  label-nav:
    fontFamily: -apple-system, BlinkMacSystemFont, "SF Pro Text", "Segoe UI", sans-serif
    fontSize: 11px
    fontWeight: 500
    lineHeight: 14px
  label-caps:
    fontFamily: -apple-system, BlinkMacSystemFont, "SF Pro Text", "Segoe UI", sans-serif
    fontSize: 11px
    fontWeight: 600
    lineHeight: 15px
    letterSpacing: 1px
rounded:
  none: 0px
  sm: 6px
  md: 12px
  lg: 16px
  xl: 20px
  full: 9999px
spacing:
  xs: 4px
  sm: 8px
  md: 12px
  base: 16px
  lg: 20px
  xl: 24px
  page-inset: 16px
  section-gap: 24px
  touch-target: 44px
  composer-height: 56px
  task-row-height: 64px
  tab-bar-height: 56px
  content-max: 430px
components:
  meeting-title:
    textColor: '{colors.on-surface}'
    typography: '{typography.headline-lg}'
  avatar:
    size: 28px
    rounded: '{rounded.full}'
  avatar-small:
    size: 16px
    rounded: '{rounded.full}'
  ai-summary:
    backgroundColor: '{colors.primary-soft}'
    textColor: '{colors.on-surface}'
    typography: '{typography.body-md}'
    rounded: '{rounded.xl}'
    padding: '{spacing.base}'
  decision-marker:
    backgroundColor: '{colors.primary-soft}'
    textColor: '{colors.primary-strong}'
    rounded: '{rounded.full}'
    size: 24px
  decision-title:
    textColor: '{colors.on-surface}'
    typography: '{typography.label-lg}'
  action-list:
    backgroundColor: '{colors.surface}'
    rounded: '{rounded.lg}'
  action-title:
    textColor: '{colors.on-surface}'
    typography: '{typography.label-md}'
  action-title-completed:
    textColor: '{colors.muted}'
    typography: '{typography.label-md}'
  checkbox:
    backgroundColor: '{colors.surface}'
    rounded: '{rounded.full}'
    size: 24px
  checkbox-checked:
    backgroundColor: '{colors.primary}'
    textColor: '{colors.surface}'
    rounded: '{rounded.full}'
    size: 24px
  badge-high:
    backgroundColor: '{colors.priority-surface}'
    textColor: '{colors.priority-text}'
    typography: '{typography.badge}'
    rounded: '{rounded.sm}'
  badge-progress:
    backgroundColor: '{colors.primary-soft}'
    textColor: '{colors.primary-strong}'
    typography: '{typography.badge}'
    rounded: '{rounded.sm}'
  badge-done:
    backgroundColor: '{colors.done-surface}'
    textColor: '{colors.done-text}'
    typography: '{typography.badge}'
    rounded: '{rounded.sm}'
  ask-ai:
    backgroundColor: '{colors.surface}'
    textColor: '{colors.on-surface}'
    typography: '{typography.body-lg}'
    rounded: '{rounded.full}'
    height: '{spacing.composer-height}'
  button-primary:
    backgroundColor: '{colors.primary}'
    textColor: '{colors.surface}'
    rounded: '{rounded.full}'
    size: '{spacing.touch-target}'
  button-primary-pressed:
    backgroundColor: '{colors.primary-strong}'
  button-primary-disabled:
    backgroundColor: '{colors.done-surface}'
    textColor: '{colors.secondary}'
  button-tertiary:
    backgroundColor: transparent
    textColor: '{colors.secondary}'
    rounded: '{rounded.full}'
    size: '{spacing.touch-target}'
  nav-item:
    backgroundColor: '{colors.surface}'
    textColor: '{colors.secondary}'
    typography: '{typography.label-nav}'
  nav-item-selected:
    backgroundColor: '{colors.surface}'
    textColor: '{colors.primary}'
    typography: '{typography.label-nav}'
---

# AI Meeting Companion

## Overview

A premium, calm productivity interface for people reviewing meeting outcomes and coordinating follow-up work. It should feel intelligent, trustworthy, and immediately scannable. The selected meeting lives within the Meetings tab.

This file follows the [Google Labs DESIGN.md alpha format](https://github.com/google-labs-code/design.md/blob/main/docs/spec.md). The supplied image is the visual source. Token values are implementation decisions inferred from that raster reference, not extracted source measurements. The YAML values are normative for this design system; the prose explains their application. Suggested interactive states extend the static image.

Use near-white surfaces, violet accents, strong titles, and compact metadata. Summary, decisions, and tasks have distinct levels of containment. Do not introduce additional visual themes or dashboard sections.

## Colors

Violet is the primary interaction and AI color. Dark ink anchors the content, while gray carries supporting information. Peach is reserved for the High badge and is not a second brand accent.

| Token | Value | Application |
| --- | --- | --- |
| `primary` | `#7540F5` | AI indicators, send button, checked controls, selected tab |
| `primary-strong` | `#6330D9` | Text on lavender and pressed primary buttons |
| `primary-soft` | `#F2EDFF` | Summary panel, numbered markers, progress badge |
| `neutral` | `#FCFCFE` | Page canvas |
| `surface` | `#FFFFFF` | Task group, composer, navigation |
| `on-surface` | `#11101A` | Titles and body copy |
| `secondary` | `#646775` | Metadata, descriptions, inactive navigation |
| `muted` | `#707481` | Placeholder and completed task title |
| `border` | `#E4E5EB` | Container outlines and list dividers |
| `control-outline` | `#858996` | Unchecked completion-control outline |
| `priority-surface` | `#FFE3DA` | High-priority badge fill |
| `priority-text` | `#9B311F` | High-priority badge text |
| `done-surface` | `#F0F0F3` | Done badge and disabled button fill |
| `done-text` | `#616472` | Done badge text |

The muted text and control outline are slightly darker than the generated image to preserve readability. Use visible text labels and checkmarks alongside color cues.

## Typography

Use the iOS system sans-serif, with the fallback stack encoded in the tokens. Preserve bold meeting and section headings, semibold task and decision titles, and regular supporting text.

| Token | Role | Size / line height | Weight |
| --- | --- | --- | --- |
| `headline-lg` | Meeting title | 28px / 34px | 700 |
| `headline-md` | Section headings | 20px / 25px | 700 |
| `label-ai` | AI summary label | 17px / 22px | 600 |
| `label-lg` | Decision titles | 16px / 21px | 600 |
| `label-md` | Task titles | 15px / 20px | 600 |
| `body-lg` | Composer input | 16px / 22px | 400 |
| `body-md` | Summary body | 15px / 21px | 400 |
| `body-sm` | Decision explanation and header timestamp | 14px / 20px | 400 |
| `caption` | Assignee, due date, participant caption | 13px / 18px | 400 |
| `badge` | Status badges | 12px / 16px | 500 |
| `label-nav` | Bottom-tab labels | 11px / 14px | 500 |
| `label-caps` | Header eyebrow | 11px / 15px | 600 |

Only the eyebrow is uppercase, with 1px tracking. Use sentence case elsewhere. Scale text with user settings and grow rows to fit; never shrink text to force the whole screen into view.

## Layout

Use this order:

1. Native iOS status bar.
2. Meeting header with title, metadata, participants, and more-options control.
3. AI summary panel.
4. Key decisions section with two numbered items.
5. Action items section with completion count and three task rows.
6. Ask AI composer.
7. Five-tab bottom navigation and native home-indicator safe area.

### Sizing and adaptation

Use a nominal **390 × 844 logical-point** viewport as a starting point. Treat the supplied image as the visual reference, not a requirement to reproduce raster pixels at their original resolution.

Use a 4px-based spacing scale: 4, 8, 12, 16, 20, and 24px. Default page insets are 16px, major section gaps 24px, and heading-to-content gaps 12px. Summary padding is 16px. Task rows have 12px vertical and 16px horizontal padding, with a 64px minimum height. The composer and tab-bar content are each 56px high; bottom safe-area space is additional.

Token dimensions use CSS `px`, as required by the format. In a native iOS implementation, map the numeric sizes to logical points, not physical screen pixels. Safe-area insets come from the device rather than fixed tokens.

Use a vertically scrollable content region. Anchor the composer above the bottom navigation, reserve its occupied space in the scroll area, and respect safe-area insets. At the reference text size, aim to show the entire overview without excessive empty space. Allow scrolling instead of shrinking text on smaller screens.


On wider displays, center a content column with a 430px maximum width. At larger text sizes, allow metadata to wrap and move badges below task titles when necessary. Keep the composer above the keyboard, and reserve enough scroll padding that it never covers a task.

## Elevation & Depth

The screen is nearly flat. Create depth with the lavender summary surface, white task grouping, subtle 1px borders in `border`, and clear spacing. Decisions remain on the page canvas without individual cards.

Use no shadow by default. If an overlay needs separation, a restrained `0 2px 8px 0 rgba(17, 16, 26, 0.03)` shadow is permitted. Do not apply it to every section. Container borders are subtle decoration; unchecked controls use `control-outline` for stronger visibility.

## Shapes

Rounded geometry makes the dense screen approachable. Apply radii by component role:

| Token | Value | Use |
| --- | --- | --- |
| `none` | 0px | Dividers and tab-bar edge |
| `sm` | 6px | Status badges |
| `md` | 12px | Small secondary surfaces if needed |
| `lg` | 16px | Grouped task container |
| `xl` | 20px | AI summary |
| `full` | 9999px | Composer, avatars, send button, numbered markers, completion circles |

Use consistent 22–24px outline icons. Avatars are circular photographic crops, with a thin white ring where they overlap. Keep the visible completion circle at 24px inside a 44px touch target.

## Components

### Meeting header

Show the eyebrow **MEETING OVERVIEW**, with a horizontal ellipsis button aligned at the trailing edge. Beneath it, place **Product sync** as the main title, followed by **Sep 10, 2026 · 10:00–10:45 AM**.

The image places an overlapping participant cluster to the right of the title area, with small circular portraits, a pale overflow circle, and the caption **Maya, Alex, Sam +2**. Use approximately 28px avatars, a small overlap, and a thin surface-colored ring.

When the title, timestamp, and participant cluster cannot fit comfortably, move participants to their own line beneath the timestamp. Do not compress or clip the title to preserve the image’s two-column arrangement.

Participant counts should come from actual meeting data. The generated reference’s portraits and overflow label are illustrative; ensure the visible portraits, overflow count, and caption agree in implementation.

### AI summary

Use one lavender rounded panel. Align a small violet sparkle icon with the label **AI summary**. Put the summary below with a compact gap.

Reference copy:

> The team aligned on the onboarding flow and confirmed the next release scope. Updated designs and final copy are due before Friday’s handoff.

Keep the text to two or three short sentences. Let the panel grow naturally; do not truncate important summary content behind a fixed height.

### Key decisions

Render **Key decisions** directly on the page background. Use two stacked items, each with a pale violet numbered circle at the leading edge and a text column to its right. Markers are approximately 24px in diameter.

| Marker | Title | Explanation |
| --- | --- | --- |
| 1 | Simplify onboarding | Use a three-step flow for new users. |
| 2 | Keep the release focused | Move dashboard changes to the next sprint. |

Use 16px between items. Avoid enclosing each decision in a separate card. Explanations may wrap on narrow screens.

### Action items

Place **Action items** on the left and **1 of 3 done** on the right of the section header. Group all three rows in one white rounded rectangle with a fine outline and separators between rows.

Each row contains a completion control, task text, an assignee-and-date metadata line, and a trailing status or priority badge. The metadata line begins with a tiny circular avatar, 16px.

| Task | Assignee | Due | Badge | Completion |
| --- | --- | --- | --- | --- |
| Update onboarding screens | Maya | Sep 11 | High | Unchecked |
| Finalize welcome copy | Alex | Sep 11 | In progress | Unchecked |
| Share meeting notes | Sam | Sep 10 | Done | Checked |

Unchecked controls are hollow circles with a `control-outline` outline. The checked control is violet with a white checkmark. Use a 24px visible circle inside a larger touch target.

Completed task titles use muted text and a strikethrough. Keep assignee and due-date information visible. Badges have compact horizontal padding and 6px corners: peach for **High**, lavender for **In progress**, and neutral gray for **Done**.

Priority and completion status are distinct data fields even though the reference displays one compact badge per row. Show **Done** for completed items, otherwise the relevant status or priority. Completing a task must not erase its stored priority.

### Ask AI composer

Use a white, lightly outlined pill spanning the content width. Place a violet sparkle at the leading edge, the exact placeholder **Ask about this meeting**, and a violet circular send button with a white paper-plane icon at the trailing edge.

Keep the text area flexible and the send target at least 44px. Do not add suggestion chips or a separate large AI card to this screen.

### Bottom navigation

Use a white surface, a fine top border, five equal-width tabs, and the native bottom safe area.

| Tab | Icon concept | Reference state |
| --- | --- | --- |
| Meetings | Calendar outline | Selected, violet icon and label |
| Notes | Document outline | Inactive, gray |
| AI | Sparkle outline | Inactive, gray |
| Tasks | Circled check outline | Inactive, gray |
| Profile | Person outline | Inactive, gray |

Use consistent outline icons of 22–24px, with labels beneath. Keep AI visually consistent with the other tabs rather than using an oversized floating button. In a native app, let iOS render the status bar and home indicator.


### Buttons and input states

The send control uses `button-primary`; the ellipsis uses `button-tertiary`. Use `button-primary-pressed` on press and `button-primary-disabled` when the question is empty or submission is in progress. Other properties inherit from the base component. Keep a visible focus ring using `primary-strong` for keyboard navigation. Use `muted` for the input placeholder and `on-surface` for entered text. Give the composer an accessible label independent of the placeholder.

Status badges are informational, not clickable filter chips. Keep their text visible in every state. Use consistent 8px horizontal and 4px vertical padding.

### Interaction guidance

These behaviors extend the static reference and are implementation guidance.

- **Task completion:** Tapping the completion control toggles completion, updates the checkmark, title treatment, badge, and section count. Allow reversal. If saving fails, restore the prior state and show a concise retry message.
- **Task details:** Tapping task text may open task details. Keep this action separate from the completion control.
- **Ask AI:** Focusing the composer opens the keyboard. Keep the input above the keyboard and temporarily hide the bottom tabs if needed. Enable submission only when trimmed text is nonempty. Submission opens a conversation scoped to this meeting.
- **AI response:** Show a loading state while answering. Use meeting evidence where available; if the discussion does not contain the answer, say so. Do not invent meeting decisions or assignments.
- **Navigation:** Tab selection updates both the icon and label state. Preserve the current meeting when returning to Meetings.
- **Participants:** A participant cluster may open a participant list.
- **More options:** Open a compact meeting-specific action menu. Include only implemented actions.
- **Motion:** Use brief, subtle state transitions, approximately 150–200 ms. Respect reduced-motion preferences.


### Loading, empty, and error states

- During loading, use restrained skeletons matching the final layout.
- If no summary exists, show a short message such as **Summary not available yet** within the summary region.
- If no decisions were found, show **No key decisions captured** beneath the section title.
- If there are no tasks, show **No action items yet** and omit the completion ratio.
- If meeting data cannot load, show a clear inline error with a retry control.
- If an AI request fails, preserve the typed question and offer retry without clearing the input.

## Do's and Don'ts

- Do preserve the seven-region screen order and select Meetings in the five-tab navigation.
- Do keep the AI summary lavender, decisions unboxed, and all tasks in one outlined group.
- Do reuse the YAML tokens and component references; avoid introducing near-duplicate colors or spacing values.
- Do keep summary copy to two or three concise sentences and use the reference content above.
- Do synchronize task completion, its visual treatment, and the completion count.
- Do retain text labels, checkmarks, and accessible selection states rather than communicating by color alone.
- Do use real buttons, labeled inputs, semantic headings, and at least 44px touch targets.
- Do preserve readable contrast for normal text and visible control boundaries; the darker muted tokens are intentional.
- Do allow scrolling and text wrapping for narrow viewports and larger text settings.
- Do respect native safe areas and reduced-motion preferences.
- Don't use heavy card treatments, decorative gradients, oversized AI buttons, or additional marketing content.
- Don't clip the title or shrink text to preserve a two-column header. Move participants below the timestamp when necessary.
- Don't hide assignees or dates on completed tasks, or erase priority when completion changes.
- Don't let the composer or navigation cover meeting content.
- Don't hard-code inconsistent participant counts from the generated avatars; derive them from meeting data.
