---
weight: 1
title: "Not All Work Belongs in the Sprint"
draft: false
---

# Not All Work Belongs in the Sprint: The Dual-Streams of Software Development

<iframe src="dual-streams.html" width="600" height="400" frameborder="0" allowfullscreen></iframe>

In agile development, we’re often focused on user stories and sprint planning, but not every task truly belongs in a sprint. **Maintenance and infrastructure work**, like security patches, framework updates, and cloud configurations, play a crucial role in keeping an application running smoothly—but these aren’t the kind of work stakeholders usually think of when they’re discussing priorities.

To keep things organized and efficient, teams should adopt a **dual-stream approach**: one stream dedicated to product features (the sprint) and another for infrastructure and maintenance work. This approach helps clarify responsibilities, ensures a smoother sprint process, and allows teams to focus on user-facing work without getting bogged down by behind-the-scenes tasks.

## Understanding the Difference: Maintenance Work vs. Sprint Work

In simple terms, maintenance work is the ongoing effort to keep an application stable, secure, and up-to-date. This can  include tasks like:
- Applying software security patches
- Managing log files and backups
- Upgrading versions of programming languages (e.g., Java) or frameworks (e.g., Spring, React)
- Configuring or updating cloud environments
- Ensuring compatibility with newer versions of phone devices and web browsers

These tasks have their own timelines and requirements, often dictated by external factors (e.g., security deadlines or platform support changes). This is usually not the type of work that the product owner would be responsible to prioritize; it’s necessary work to keep the application operational, regardless of whether stakeholders request new features.

In contrast, **sprint work** is about delivering value to the user—enhancements, new features, and improvements that stakeholders have asked for and prioritized.

#### The Right Work for the Right Stream

When the stakeholders say, “Just keep the application up and running smoothly,” they’re describing a maintenance state. Maintenance work ensures that everything continues working without interruption, even if no new features are added. But when stakeholders say, “We want these new features,” they’re asking for product development, which is where sprints come in.

Using a dual-stream approach, we can:
1. Keep maintenance tasks in an infrastructure/maintenance stream, ensuring that necessary updates don’t clutter the sprint backlog.
2. Focus the sprint stream on work that the product owner has explicitly prioritized, enabling the team to deliver valuable features without distractions.

## Handling Infrastructure as a Pre-Condition for Sprint Work

Sometimes, infrastructure work must be completed before a user story can be implemented. For example, to build a new feature, the team might need to:
- Set up new environments or tools
- Upgrade the framework to the latest version
- Acquire additional resources or access

In these cases, the infrastructure work can be linked as a **blocker** to the user story. This way, the story will remain in the backlog until it's unblocked, allowing the team to negotiate with stakeholders and set expectations. It’s clear that the infrastructure work isn’t being prioritized by the product owner but is required to complete the story effectively.

## Advantages of Separating Infrastructure/Maintenance from the Sprint

1. **Less Burden on the Product Owner**: Product owners don’t need to prioritize tasks they don’t fully understand or request directly. They can focus on user-facing features without getting bogged down by the technicalities of infrastructure.

2. **Cleaner Backlog**: By keeping maintenance and infrastructure tasks out of the sprint backlog, teams can keep the backlog focused and easier to manage.

3. **Accurate Story Estimations**: Infrastructure work often has unpredictable timelines and dependencies. By keeping it separate, user story estimations aren’t disrupted by factors outside the team’s immediate control.

4. **Fewer Dependencies**: With infrastructure work happening outside of the sprint, the team faces fewer dependencies that could delay user stories or cause sprint bottlenecks.

5. **Better Planning and Negotiation**: When infrastructure tasks are separate, the team can negotiate timelines for this work before bringing related user stories into the sprint. Stakeholders are assured that any infrastructure work won’t impact their priorities unless absolutely necessary.

6. **Reduced Sprint Disruptions**: Sometimes, project managers or product owners can help expedite infrastructure work ahead of a sprint, allowing the sprint team to work with fewer obstacles and at a consistent pace.

Ultimately, the sprint stream should focus on what the product owner wants to prioritize, while infrastructure tasks should stay in the maintenance stream to support these priorities without cluttering the sprint.

## A Real-Life Example: Maintenance Mode and Resuming Sprints

Imagine a scenario where an application was completed and has been running smoothly in maintenance mode for over a year. Now, stakeholders have approved funding to add a new set of features. Often, teams will jump straight into running sprints, but this isn’t always ideal. Using a dual-stream approach, the team could strategically choose to first:
- Upgrade to the latest programming language or platform version.
- Update frameworks, libraries, and databases.
- Address technical debt or refactor code as needed.

This preparation creates a strong foundation for the new sprint work. The team can enter sprints with up-to-date tools, increased speed, and the ability to use new framework features. Without this step, the team might face limitations or potential bugs due to outdated software.

## Example: Framework Upgrade to Enable a New Feature

Another common scenario is when a product owner requests a small improvement—say, an additional feature on a calendar widget. However, the calander widget is part of a package collection of widget and so it would require that the package and entire collection of widgets be upgraded in one go. Sometimes, to avoid dealing with this infrastructure work, developers might just leave the old collection in place and find a standalone widget to work around the issue. But this workaround can lead to inconsistencies in the look-and-feel, technical debt as the collection continues to fall behind the latest release version, and future maintenance headaches.

Instead, using the dual-stream approach, the team could identify the framework upgrade as maintenance work and complete it before starting the sprint. This allows the sprint to focus on real feature work, with access to the latest framework capabilities and better support options.

## Conclusion: Embracing the Dual-Stream Approach

When teams separate sprint work from infrastructure and maintenance, they gain clarity, control, and flexibility. The team has an ongoing infrastructure/maintenance stream where essential technical tasks happen, independent of the sprint planning. Once the foundational work is complete, the team can begin sprinting at full capacity, delivering the new features that the product owner and stakeholder are requesting.

When deciding where a task belongs, consider:
- Is this something the product owner requested and can understand how to prioritize?
- Can this work be described in a user story and completed within a sprint?
- Or is this work required to maintain, support, and keep the the application running smoothly?

By keeping infrastructure and maintenance tasks separate, agile teams can focus sprints on meaningful product work, ensuring a smoother process, better stakeholder alignment, and fewer unexpected hurdles.
