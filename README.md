# Checkpoint5-Approach shelf

## Introduction
<p>The goal of this project is to create a program that allows RB-1 robot to approach, detect, and attach a warehouse shelf.</p>

## Pre Approach
<p>The robot moves to the loading position. This requires two parameters- 1. obstacles: distance the robot will stop and 2. degrees: rotation the robot will turn to the shelf.</p>

    ros2 launch attach_shelf pre_approach.launch.xml obstacles:=0.3 degrees:=-90

## Final Approach
<p>The robot will detect the shelf using laser intensity. If found, the robot will move toward the shelf and finally lift the shelf.</p>

    ros2 launch attach_shelf attach_to_shelf.launch.py obstacle:=0.3 degrees:=90 final_approach:=True
