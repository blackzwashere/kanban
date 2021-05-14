---
layout: story
title: SPIKE Kanban Layout
date: 2016-03-16 11:04

acs:
 - determine a technology on which to base a Kanboard board

assigned:
 - Luther Baker
 - John Doe

scenarios:
 - As a developer, I would like to see Stories laid out on a Kanban board to help determine if the selected technology will scale and work in general for the application.

usecases: [["UC001 Kanban Visual", "2016-03-17-uc001-kanban-visual"]]

---

Build a simple grid view to represent columns for a Kanban board. Consider a [UICollectionView](https://developer.apple.com/library/ios/documentation/UIKit/Reference/UICollectionView_class/) with a custom [UICollectionViewLayout](https://developer.apple.com/library/ios/documentation/UIKit/Reference/UICollectionViewLayout_class/).
