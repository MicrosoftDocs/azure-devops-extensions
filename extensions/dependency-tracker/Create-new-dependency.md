---
title: Create a dependency
description: Learn how to create dependency in the Dependency Tracker extension for Azure DevOps.
author: cherylsingh
ms.author: chesing
ms.topic: conceptual
ms.date: 02/23/2024
---

# Create a dependency with Dependency Tracker

Enable users to plan and manage dependencies across areas by providing a clear visual of all dependencies a team is consuming and producing in Azure DevOps. Use Dependency Tracker to create these dependencies.

## Prerequisites
- Download the [Dependency Tracker extension](https://marketplace.visualstudio.com/items?itemName=ms-eswm.dependencytracker) for Azure DevOps in the [Visual Studio Marketplace](https://marketplace.visualstudio.com/).
- Ensure each team tracks their work in their designated area path. This ensures that both teams maintain their own context and focus. For example, Team A and Team B might have separate area paths where they manage their tasks.
- Identify work items that are interdependent between the teams. For example, Team A has a task (Task A) that depends on Team B’s work (Task B).

## Create a dependency
Do the following steps to create a dependency.

1. Sign in to your project (```https://dev.azure.com/{Your_Organization/Your_Project}```).
2. Select **Boards** > **Dependency Tracker**.
3. Select **+ New Dependency**.
  - Enter the **Producer** and **Consumer** work item IDs in the search boxes, or **Create New** work items.
    - The Producer is the team that commits to deliver the work. 
    - The Consumer is the team that needs or is dependent on the work.
      For example,
      - From Team A (Producer/predecessor): Add a successor link to Task A. This signifies that Task A must finish before Task B can begin.
      - From Team B (Consumer/dependent): Add a predecessor link to Task B. This indicates that Task B cannot start until Task A is completed.

  > [!div class="mx-imgBorder"]  
  > ![Screenshot of Dependency Tracker creation window.](../images/Easy-Button.png)

4. Select **Save**.

   Your dependency saves.

   You can also create dependencies from the **Links** tab.

   > [!div class="mx-imgBorder"]  
   > ![Screenshot of Dependency Tracker, links view.](../images/Links-View.png)

## Related articles

- [Overview of Dependency Tracker](overview.md)
- [Dependency views](dependency-views.md)
- [Dependency Timeline](timeline.md)
- [Dependency Risk Graph](risk-graph)
