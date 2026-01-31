---
name: ios-hig-design
description: 'Design native iOS apps following Apple''s Human Interface Guidelines. Use this skill when building iPhone/iPad interfaces, creating SwiftUI/UIKit components, validating iOS design compliance, or ensuring accessibility. Covers layout, typography, navigation, components, gestures, colors, and platform conventions.'
license: MIT
metadata:
  author: wondelai
  version: "1.0"
---

# iOS Human Interface Guidelines Design Skill

This skill guides creation of native iOS app interfaces that feel intuitive, consistent, and aligned with Apple's design philosophy.

## Core Design Principles

Apple's iOS design philosophy rests on three foundational principles:

### 1. Clarity
Every element must be legible and purposeful. Typography, iconography, and spacing communicate hierarchy and focus.

### 2. Deference
The interface should never overshadow the content. The UI exists to support user tasks, not distract from them.

### 3. Depth
Layering, transitions, and realistic motion provide hierarchy and spatial relationships.

## Scoring

**Goal: 10/10.** When reviewing or creating iOS interfaces or SwiftUI/UIKit code, rate them 0-10 based on adherence to the principles below. A 10/10 means full alignment with all guidelines; lower scores indicate gaps to address. Always provide the current score and specific improvements needed to reach 10/10.

---

## Screen Sizes & Layout

### iPhone Screen Sizes (Design Points)

| Device | Frame Size | Export Scale |
|--------|-----------|--------------|
| iPhone 15 Pro Max, 14 Pro Max | 430 × 932 | @3x |
| iPhone 15 Pro, 15, 14 Pro | 393 × 852 | @3x |
| iPhone 14, 13, 12 | 390 × 844 | @3x |
| iPhone SE (2nd/3rd gen) | 375 × 667 | @2x |

**Best Practice**: Design for smaller screens first (375pt width).

### Page Layout Structure

```
┌─────────────────────────────────┐
│         Status Bar (59pt)       │
├─────────────────────────────────┤
│         Nav Bar Row 1 (44pt)    │
├─────────────────────────────────┤
│         Nav Bar Row 2 (58pt)    │  ← Large title (optional)
├─────────────────────────────────┤
│         Content Area            │
├─────────────────────────────────┤
│         Tab Bar (49pt)          │
├─────────────────────────────────┤
│       Home Indicator (34pt)     │
└─────────────────────────────────┘
```

### Safe Areas

**Critical**: UI components must not overlap with hardware features (notch, Dynamic Island, home indicator).

```swift
VStack { Text("Content") }  // Default: respects safe area

VStack { Color.blue }.ignoresSafeArea()  // Extend beyond
```

---

## Quick Reference: Component Spacing

```
Touch Target Min:     44 × 44pt
Screen Edge Margin:   16-20pt
List Row Height:      44pt minimum
Standard Spacing:     8 / 16 / 24pt
```

---

## Common Pitfalls

**Don't:**
- Override standard gestures (swipe back, pull refresh)
- Use touch targets smaller than 44pt
- Ignore safe areas
- Force Android patterns (top tab bar, hamburger menus)
- Neglect Dark Mode
- Use low contrast text

**Do:**
- Use native components
- Test on real devices
- Support Dynamic Type
- Test with VoiceOver enabled
- Preview in both light and dark modes

---

## Detailed Reference Files

**Core Design:**
- [references/typography.md](references/typography.md) — Text styles, font sizes, Dark Mode typography
- [references/navigation.md](references/navigation.md) — Tab bar, navigation bar, modals, search patterns, split views
- [references/components.md](references/components.md) — Buttons, lists, input controls, menus, confirmation dialogs
- [references/colors-depth.md](references/colors-depth.md) — Semantic colors, Dark Mode, contrast ratios
- [references/gestures.md](references/gestures.md) — Standard gestures, haptics, animations
- [references/accessibility.md](references/accessibility.md) — VoiceOver, Dynamic Type, checklist
- [references/app-icons.md](references/app-icons.md) — Icon sizes, shape, guidelines

**Input & System Integration:**
- [references/keyboard-input.md](references/keyboard-input.md) — Keyboard types, input accessory views, hardware keyboard support
- [references/privacy-permissions.md](references/privacy-permissions.md) — Permission request timing, pre-permission screens, handling denial
- [references/widgets-extensions.md](references/widgets-extensions.md) — Widget sizes, App Clips design, Live Activities
- [references/system-integration.md](references/system-integration.md) — Siri, Shortcuts, Handoff, drag-drop, universal links

---

## Resources

- [Apple Human Interface Guidelines](https://developer.apple.com/design/human-interface-guidelines/)
- [SF Symbols](https://developer.apple.com/sf-symbols/)
- [Apple Design Resources (Figma/Sketch)](https://developer.apple.com/design/resources/)
- [WWDC Design Sessions](https://developer.apple.com/videos/design/)
