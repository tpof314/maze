# 用Python生成迷宫的源代码

## 算法简介

1. 生成一张网格，把网格里面的所有**边**都存进一个列表**edgeList**里面.
2. 从(0, 0)开始，做DFS。每次DFS的时候，随机地选择四周一个没有走过的格子，凿墙过去，把道路打通。凿墙的时候，把**edgeList**列表中相对应的那堵墙删除掉。
3. 将剩下的没有凿开过的墙画出来，就是一个完整的迷宫了。

---

# Generate a maze using Python

## A Brief Description of the Algorithm

1. Generate a grid of a given width and height. Save all the edges into list named **edgeList**.
2. Starting from the cell `(0, 0)`, perform a DFS search. In each step, randomly pick a unvisited neighbour cell, and break the wall in between. More specifically, when breaking the wall, what we need to do is just to remove the corresponding edge from the **edgeList**.
3. Sketch all the rest edges in the **edgeList** and then we may get a maze.

