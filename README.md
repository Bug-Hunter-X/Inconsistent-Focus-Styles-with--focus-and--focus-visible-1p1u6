# Inconsistent Focus Styles with :focus and :focus-visible

This repository demonstrates a common issue encountered when using the `:focus-visible` pseudo-class in CSS alongside existing `:focus` styles. The interaction between these pseudo-classes can lead to unexpected visual results and potential accessibility problems.

The `bug.css` file showcases the problematic CSS code, resulting in inconsistent and possibly confusing focus states.  The `bugSolution.css` file provides a solution demonstrating how to address this issue and achieve a more consistent and accessible focus experience.

## Problem
The primary issue arises from the combination of a custom focus style (`box-shadow`) and the `:focus-visible` pseudo-class. While intended to enhance keyboard navigation accessibility, it can clash with existing focus styles. It might also fail to consistently override a default browser focus outline, leading to overlapping styles.

## Solution
The solution involves careful ordering and specificity of CSS rules to ensure the desired focus behavior is consistently applied.  This often means ensuring that the `:focus-visible` style is prioritized in cases of conflict, or potentially using a more robust focus management technique to avoid unintended style overlaps.