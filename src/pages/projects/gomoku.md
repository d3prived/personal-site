---
layout: ../../layouts/ProjectLayout.astro
title: Gomoku / 5 In a Row
description: An interactive gomoku (5 in-a-row) AI
tags: ["Go", "TypeScript", "React.js", "Concurrency", "AI"]
githubUrl: https://github.com/rudrowo/5-in-a-row
timestamp: 2023-06-24T02:39:03+00:00
featured: false
filename: gomoku
---

## An AI built using the Minimax Algorithm with Alpha-Beta Pruning

![](/gomoku_peek.gif)

## Technologies used:

- [React](https://reactjs.org/)
- [Gin Framework (Go)](https://gin-gonic.com/)

## How it works

- I split the 10x10 board into 36 smaller boards- each having dimension 5x5.
- Run min-max algorithm on each of the smaller boards concurrently.
- Compare the scores of each smaller board and choose the board that gives the AI the highest chance of winning.

![Architecture diagram](/gomoku_arch.svg)
