🛰️ **3D Subsurface Visualization via Geospatial AI (Synthetic Data)**
This project provides a high-quality implementation of a 3D subsurface modeling and visualization tool using synthetic geospatial data. It combines AI-powered segmentation, interactive 3D plotting, and Excel export to simulate a professional geospatial analytics pipeline.

🚀 **Features**
✅ Synthetic 3D geological data generation

✅ AI-powered segmentation using K-Means clustering

✅ High-quality interactive 3D visualization (via Plotly)

✅ Excel export for use in GIS or ML pipelines

✅ Clean, modular, production-ready Python structure

📁 File Structure
bash
Copy
Edit
subsurface_visualization/
├── subsurface_visualizer.py         # Main module: generation, clustering, and visualization
├── synthetic_subsurface_sample.xlsx # Sample Excel export with synthetic data
├── README.md                        # Project documentation
🧪 Dependencies
Install required Python packages with:

bash
Copy
Edit
pip install numpy pandas plotly scikit-learn openpyxl
🧠 How It Works
1. Synthetic Data Generation
A 3D grid is created and populated with sinusoidal and noise-modulated values to simulate subsurface geological variability.

2. AI Segmentation
Using K-Means clustering, values are categorized into discrete "material" types such as rock layers or soil types.

3. 3D Visualization
Interactive 3D scatter plots are rendered using Plotly, with depth visualized as a reversed Z-axis.

4. Excel Export
Data is flattened and saved to .xlsx, making it compatible with GIS software, spreadsheets, or further ML workflows.

🖥️ Example Usage
python
Copy
Edit
from subsurface_visualizer import SubsurfaceVisualizer

# Step 1: Initialize
vis = SubsurfaceVisualizer(nx=60, ny=60, nz=30)

# Step 2: Generate synthetic geology
vis.generate_synthetic_data()

# Step 3: AI segmentation
vis.segment_layers(n_clusters=5)

# Step 4: 3D visualization
vis.plot_3d_scatter(use_segmentation=True, save_html=True)

# Step 5: Export to Excel
vis.export_to_excel(filename="subsurface_data.xlsx", use_segmentation=True)
📊 Output Example
subsurface_data.xlsx

Columns: Longitude, Latitude, Depth, Value or Cluster

Optional: Interactive .html file with 3D scatter viewer

👤 Author
Tarinabo williamtarinabo@gmail.com
