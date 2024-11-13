---
weight: 1
title: "QA as Part of Development"
draft: false
---

# QA as Part of Development

One common pitfall in agile teams is treating Quality Assurance (QA) as a step that follows development rather than making it part of the development itself. The reality? Quality needs to be a priority from day one, baked right into the development process.

Let’s dive into why QA should be woven into the fabric of development—and how this approach can help your team deliver higher-quality work without the stress of last-minute testing and fixes.

## Quality Isn’t an Afterthought—It’s an Integral Part of Development

Quality should be part of every development conversation. As the team clarifies what needs to be done to complete a user story, they should also discuss:
- How they’ll ensure the work meets quality standards.
- How they’ll confirm the new feature functions as intended through rigorous testing.

With this proactive approach, developers and QA can plan for quality right from the start, pinpointing the areas that need close attention. This doesn’t just improve the final product; it also provides developers with insights into potential risks and unique scenarios they might not consider on their own.

## Example: Considering Shared Code for Multiple Languages

Imagine your team is working on an app with both English and German versions. While much of the app’s logic might be shared across both languages, there may be cases where the code differs slightly between the two. If the development and QA teams work together from the outset, they can establish where testing is needed for each language:
- **Shared Logic**: If English and German versions share the same code for a particular feature, it might only need testing once.
- **Separate Implementations**: If there are two separate codebases for English and German, both will need thorough testing to ensure they’re fully functional.

By bringing QA into the development process, you get a clear understanding of where testing is essential and where it’s redundant—streamlining the process and minimizing duplicate effort.

## Catching Edge Cases and Exceptional Scenarios Early

Experienced QA professionals are invaluable when it comes to spotting edge cases that developers might overlook. For instance, they might ask:
- “What happens if the database is down? Will the app handle it gracefully, or does it assume the database will always be available?”
- “How does the application work if a user’s keyboard is set to a right-to-left language, like Arabic or Hebrew?”
- “Can the app handle email addresses with special characters, like emojis in domain names?”

By bringing these questions up early in development, QA helps the team account for unusual but realistic scenarios before they become issues. Addressing these potential pain points before they turn into real bugs saves everyone time and energy.

## Real-Time Collaboration Between Developers and QA

When QA is involved throughout the development process, they can often catch issues as code is being written. If a QA expert notices a potential problem, they can discuss it with the developer immediately, while the code is fresh in their mind. This is a far more efficient approach than waiting until the story is marked “done,” only to find that there’s an issue that requires revisiting code from weeks prior.

With QA input at every stage of development, teams can resolve issues faster, with fewer context-switching costs. Developers and QA work together, side by side, to ensure that each user story meets the agreed-upon standards.

## Shared Responsibility for High-Quality Code

Ultimately, developers and QA should collaborate on quality. They both play an essential role in delivering robust, dependable features that meet user needs. When quality is a team responsibility, it fosters a shared commitment to high standards and a sense of pride in delivering work that’s reliable from the get-go.

**Key Takeaway**: By making QA an integral part of development rather than a post-development step, teams can catch issues early, streamline testing, and ensure they’re building high-quality software from the very start. Agile is all about adapting and improving, so let’s adapt by treating quality as part of development, not something left for later.

