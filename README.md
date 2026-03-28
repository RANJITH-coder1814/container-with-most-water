# container-with-most-water
Given an array height where each element represents the height of a vertical line, find two lines that together form a container such that it holds the maximum amount of water.  You cannot tilt the container.
💧 Container With Most Water
📌 Problem Statement

Given an integer array height of length n, where each element represents the height of a vertical line, find two lines that together with the x-axis form a container such that the container holds the maximum amount of water.

⚠️ You may not tilt the container.

🧠 Approach (Two Pointer Technique)

To solve this efficiently, we use the Two Pointer approach:

Start with two pointers:
left = 0
right = n - 1

Calculate area using:

area = min(height[left], height[right]) * (right - left)
Move the pointer with the smaller height inward
Keep track of the maximum area
