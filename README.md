# Simple rosbag2 preview

## Overview

This is a lightweight, browser‑based tool to quickly preview the contents of a ROS2 bag database file (`*.db3`). It lists all available topics in the bag and provides simple per‑topic statistics such as message count, time span, and estimated frequency.

The tool is implemented as a single HTML+JavaScript file. No server or ROS2 environment is required. Everything runs locally in your browser using [sql.js](https://sql.js.org/) to read the SQLite database format used by rosbag2.

## Quick Start

👉 [Open Simple ROS2 Bag Preview](https://covao.github.io/simple_rosbag2_preview/simple_rosbag2_preview.html)

## Usage

1. Open the HTML file (`simple_rosbag2_preview.html`) in a modern web browser (tested on Chrome/Firefox).
2. Drag & drop a ROS2 bag `*.db3` file into the drop area **or** click the **Select File** button.
3. Once loaded, the tool displays:

   * A list of topics with their names and types
   * File information (name, size)
   * Topic statistics (click a topic row to view count, duration span, and approximate publishing rate)
