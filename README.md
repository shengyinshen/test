# Michigan Traffic Lab Map toolkit (MiMap)

<!-- ABOUT THE PROJECT -->
## About the Project

[![Product Name Screen Shot][product-screenshot]](https://example.com)

This MiMap toolkit allows you to load, parse, and visualize the OpenStreetMap data.

Developed by   

Features:
- Load the OpenStreetMap data to a customized [network class](network-class-label).
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

This is an example of how you may give instructions on setting up your project locally.
To get a local copy up and running follow these simple example steps.


### Prerequisites

This is an example of how to list things you need to use the software and how to install them.
* npm
  ```sh
  npm install npm@latest -g
  ```

### Installation

1. Get a free API Key at
2. Clone the repo
   ```sh
   git clone https://github.com/your_username_/Project-Name.git
   ```
3. Install NPM packages
   ```sh
   npm install
   ```
4. Enter your API in `config.js`
   ```JS
   const API_KEY = 'ENTER YOUR API';
   ```




<!-- USAGE EXAMPLES -->
## Usage

Use this space to show useful examples of how a project can be used. Additional screenshots, code examples and demos work well in this space. You may also link to more resources.

Run a demo
   ```sh
   curl -H "X-API-KEY: TESTING" http://localhost:5000/run
   ```

For more examples, please refer to the [Documentation](https://www.atlassian.com/software/confluence)




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

Project Link: [https://github.com/your_username/repo_name](https://github.com/your_username/repo_name)



<!-- MARKDOWN LINKS & IMAGES -->

[product-screenshot]: images/screenshot.png
