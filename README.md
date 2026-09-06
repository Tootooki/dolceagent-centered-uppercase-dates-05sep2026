# DOLCE AGENT — Centered Uppercase Dates

Based on `dolceagent-data-row-guide-05sep2026`.

Both date boxes display uppercase dates such as AUG 7, 2026, centered horizontally and vertically. A consistent display label sits beneath each full-size native date input so iPhone date rendering cannot push the visible text to the top. The date picker, minimum/maximum dates, required values, accessible names and validation remain native.

Display labels use ISO date components directly, avoiding timezone shifts. Presets, committed edits and input drafts update the labels. Draft typing does not change the table until committed. Keyboard editing reveals native date segments; touch and blur return to the centered label. Error coloring and focus indication remain visible.

Verification: 25 existing unit checks, 3 date-model tests and 4 focused integration tests passed. Date integration checks used a negative UTC offset and covered month/year boundaries, draft and error recovery, native editing and accessibility. Browser inspection at 320px and 393px confirmed equal 44px boxes, uppercase labels centered within 0.11px, and working date edits and presets. Physical iPhone rendering has not been directly verified.

The shared menu slider, data-row resize guide and other existing features are preserved.

Publish with `npm run publish`.
