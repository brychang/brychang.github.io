---
layout: post
title: "Islet Classification"
author: "Bryan Chang"
date: 2025-01-15 11:12:00 -0000
tags:
  - islets
categories: journal
---

I need to classify cells in 3D confocal images into the various types of islet cells. Initially, I tried applying a random forest classifier on the volume of each cell and the mean intensity of each of the four channels. Then I tried applying log1p, UMAP, then KNN classification. Both methods incorrectly classify cells in the core of large islets because insulin stains fail to fully penetrate the islet core.

Today, I will attempt to resolve the issue by providing a new feature to the classifier. This feature will provide each cell with context about its immediate neighbors.
