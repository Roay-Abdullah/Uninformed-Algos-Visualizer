<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>README - Uninformed Search Visualizer</title>
    <style>
        body {
            font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, Arial, sans-serif;
            line-height: 1.6;
            color: #24292e;
            max-width: 800px;
            margin: 40px auto;
            padding: 0 20px;
            background-color: #ffffff;
        }
        h1 { border-bottom: 1px solid #eaecef; padding-bottom: 0.3em; }
        h2 { border-bottom: 1px solid #eaecef; padding-bottom: 0.3em; margin-top: 24px; }
        code {
            background-color: rgba(27, 31, 35, 0.05);
            border-radius: 3px;
            font-family: "SFMono-Regular", Consolas, "Liberation Mono", Menlo, monospace;
            padding: 0.2em 0.4em;
        }
        pre {
            background-color: #f6f8fa;
            border-radius: 3px;
            padding: 16px;
            overflow: auto;
            line-height: 1.45;
        }
        .emoji { font-style: normal; }
        .footer { margin-top: 50px; font-size: 0.8em; color: #6a737d; text-align: center; }
        table { border-collapse: collapse; width: 100%; margin: 20px 0; }
        table, th, td { border: 1px solid #dfe2e5; }
        th, td { padding: 10px; text-align: left; }
        th { background-color: #f6f8fa; }
    </style>
</head>
<body>

    <h1>Uninformed Search Algorithms Visualizer</h1>
    <p>A Python-based interactive tool built with <code>Tkinter</code> to visualize how various Uninformed Search strategies navigate a 10x10 grid with obstacles.</p>

    

    <h2>🚀 Features</h2>
    <ul>
        <li><strong>Real-time Animation:</strong> Watch the frontier expand and nodes transition from "waiting" to "explored."</li>
        <li><strong>Algorithm Suite:</strong> Includes BFS, DFS, UCS, DLS, IDDFS, and Bidirectional Search.</li>
        <li><strong>Weighted Pathfinding:</strong> Uniform Cost Search (UCS) utilizes randomized weights displayed directly on the grid.</li>
        <li><strong>Interactive Controls:</strong> Toggle algorithms, clear paths, and view expansion order via a sidebar.</li>
    </ul>

    <h2>🛠️ Prerequisites & Installation</h2>
    
    <h3>1. System Requirements</h3>
    <p>This project requires <strong>Python 3.x</strong>. Most systems include <code>Tkinter</code> by default, but if you encounter an error, follow these steps:</p>
    
    <ul>
        <li><strong>Linux (Ubuntu/Debian):</strong> <code>sudo apt-get install python3-tk</code></li>
        <li><strong>Windows/macOS:</strong> Included with standard Python installations.</li>
    </ul>

    <h3>2. Setup</h3>
    <pre><code># Clone the repository
git clone https://github.com/yourusername/search-visualizer.git

# Navigate to the directory
cd search-visualizer

# (Optional) If you plan to extend this with Pygame:
pip install pygame</code></pre>

    <h2>🏃 How to Run</h2>
    <p>Simply run the Python script from your terminal or IDE:</p>
    <pre><code>python main.py</code></pre>

    <h2>📖 Grid Legend</h2>
    <table>
        <tr>
            <th>Color</th>
            <th>Meaning</th>
        </tr>
        <tr>
            <td><span style="color: green;">●</span> <strong>Green</strong></td>
            <td>Start Position</td>
        </tr>
        <tr>
            <td><span style="color: blue;">●</span> <strong>Blue</strong></td>
            <td>Target Goal</td>
        </tr>
        <tr>
            <td><span style="color: black;">●</span> <strong>Black</strong></td>
            <td>Static Obstacles (Walls)</td>
        </tr>
        <tr>
            <td><span style="color: #ffd700;">●</span> <strong>Yellow</strong></td>
            <td>Frontier (Nodes currently in queue/stack)</td>
        </tr>
        <tr>
            <td><span style="color: #ffcc66;">●</span> <strong>Orange</strong></td>
            <td>Explored Nodes</td>
        </tr>
        <tr>
            <td><span style="color: purple;">●</span> <strong>Purple</strong></td>
            <td>Final Optimal Path</td>
        </tr>
    </table>

    

    <h2>📝 Algorithms Included</h2>
    <ul>
        <li><strong>BFS:</strong> Guarantees the shortest path in unweighted grids.</li>
        <li><strong>DFS:</strong> Explores as deep as possible; not optimal, but memory efficient.</li>
        <li><strong>UCS:</strong> Finds the cheapest path based on cell weights.</li>
        <li><strong>IDDFS:</strong> Combines DFS memory efficiency with BFS optimality.</li>
        <li><strong>Bidirectional:</strong> Searches from both ends to meet in the middle, significantly reducing the search space.</li>
    </ul>

    <div class="footer">
        <p>Created for AI Pathfinding Education | 2026</p>
    </div>

</body>
</html>
