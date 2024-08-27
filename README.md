# TC² Meshtastic Range Test Map

### Installation

1. Clone the repository:

   ```sh
   cd ~
   git clone https://github.com/TheCommsChannel/mesh-rangetest-map.git
   cd mesh-rangetest-map
   ```
   Or download the zip file from the green "Code" button above if on Windows

2. Set up a Python virtual environment:

   ```sh
   python -m venv venv
   ```

3. Activate the virtual environment:

   - On Windows:

   ```sh
   venv\Scripts\activate
   ```

   - On macOS and Linux:

   ```sh
   source venv/bin/activate
   ```

4. Install the required packages:

   ```sh
   pip install -r requirements.txt
   ```

### Usage

1. Run Range Tests and place the csv files in the same directory. Change the name of the csv files to something that makes sense.

2. Navigate to the `mesh-rangetest-map` directory if you're not already there and activate the virtual environment:

   - On Windows:

   ```sh
   venv\Scripts\activate
   ```

   - On macOS and Linux:

   ```sh
   source venv/bin/activate
   ```
3. Run the script with the following command:

   ```sh
   python rtmap.py
   ```

3. An HTML file named rangetest-map.html will be generated which can now be opened to view the range test results.

#### Arguments

##### `-e` `--exclude`

GPS coordinate square to filter from display `<top-left>:<bottom-right>`

Note: use `--exclude='<val>'` if top is a negative value.
