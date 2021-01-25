# Michigan Traffic Lab Map Toolkit (MiMap)

<!-- ABOUT THE PROJECT -->
## About the Project

[![Product Name Screen Shot][product-screenshot]](https://example.com)

This MiMap toolkit allows you to load, parse, and visualize the OpenStreetMap data.

Developed by   

Features:
- Load the OpenStreetMap data to a customized network class
- Map data processing:
    - Convert the undirected OSM ways to directed segments
    - Split ways that traverse intersections
    - Load or infer (if not) the lane usage (dedicated left/right-turn, turning bay, etc.)
    - Identify the movements and phases in signalized intersection
    - Build the complete connections between road segments (as well as the conflict points in unsignalized/signalized intersections)
- Output the (processed) map data to osm/shapefile
- An easy map data visualization platform based on Leaflet/mapbox, see demostration [[here]](https://xingminw.github.io/osm-map-toolkit/map.html).



<!-- GETTING STARTED -->
## Getting Started

### Instal package

1. Clone the repo to the local (wherever is convenient) by running:
```
git clone https://github.com/michigan-traffic-lab/osm-map-toolkit
```
2. Go to the local folder:
```
cd osm-map-toolkit
```
3. Create (or activate) the conda environment you want to install this package:
```
conda create -n $env_name python=3.8
conda activate #env_name
pip install e .
```

### Install fast-map-matching (optional)

The map matching implementation is relied on a thrid-party implementation [[fmm]](https://github.com/cyang-kth/fmm). It was only tested in Linux (Ubuntu) system. The installment documentaiton can be found at: [[fmm-wiki]](https://fmm-wiki.github.io/). There are two additional things need more consideration: 

1. Remove the Python 2.7 REQUIRED in the cmakelist file located at [```fmm/python/CMakeLists.txt```](https://github.com/cyang-kth/fmm/blob/master/python/CMakeLists.txt). Just delete the ```2.7``` in line 10 and line 11.
2. Change the cmake prefix, in my Linux system and conda environment, I use:
```
cmake .. -DCMAKE_INSTALL_PREFIX=/home/xingminw/Anaconda3/envs/fmm
```


<!-- USAGE EXAMPLES -->
## Usage

Run a demo
   ```sh
   mimap.build_network_from_xml(file_name, verbose=True)
   ```

For more examples, please refer to the [Documentation](https://xingminw.github.io/osm-map-toolkit/build/html/index.html)




<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request



<!-- LICENSE -->
## License

Distributed under the MTL License. See `LICENSE` for more information.



<!-- CONTACT -->
## Contact

Henry Liu - henryliu@umich.edu

Project Link: [https://github.com/michigan-traffic-lab/osm-map-toolkit](https://github.com/michigan-traffic-lab/osm-map-toolkit)



<!-- MARKDOWN LINKS & IMAGES -->

[product-screenshot]: images/screenshot.png
