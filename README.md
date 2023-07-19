# Leetcode 435. Non-overlapping Intervals (Medium)

# Problem

Given an array of intervals intervals where intervals[i] = [starti, endi], return the minimum number of intervals you need to remove to make the rest of the intervals non-overlapping.

# Solution

Sort the List by end date of each interval
set the current end date to the first intervals end. Now iterate through the rets of the list, if the start date is before this end date, then it needs to be removed, increase removals by 1. Otherwise that interval is added and set its end date to the new end date. Return number of removals.
