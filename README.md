🕳️ Crack Segmentation & Path Planner 🚧
Automatic crack detection and optimal spray path generation for road repair robots.

✨ Features
🔍 Crack Detection: U-Net ML model for segmentation
🧼 Denoising: Morphological operations for clean outputs
🛠️ Path Optimization: TSP-based routing with thickness adaptation
🔄 Smoothing: DMA + Spline interpolation for smooth trajectories
🎨 Visualization: Heatmaps, directional arrows, gap detection

🚀 Quick Start
bash
Copy
# Install dependencies  
pip install tensorflow opencv-python scikit-learn networkx matplotlib  

# Run pipeline  
python main.py --input ./raw_images --output ./results
🧮 Key Parameters
Parameter	Default	Description
num_cluster	200	K-Means clusters for TSP
gap_threshold	0.5	Black pixel ratio for jumps
curvature_multiplier	4	Smoothing aggressiveness
📂 Example Workflow
raw_images/ → Resize → resized/

Segment → segmented/

Denoise → denoised/

Generate path → results/path_visualization.jpg

🌟 Next Steps
🚧 Dynamic speed control | 🔄 Buffer zones | 🤖 ROS integration

