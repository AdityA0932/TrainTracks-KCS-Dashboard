# TrainTracks: KCS Dashboard

TrainTracks is a Dash-based web application that provides a comprehensive dashboard for managing and viewing data from a MySQL database. Designed specifically for Kalva Carshade  (KCS), this tool efficiently tracks various dates associated with train components, streamlining the maintenance and management process.

## Features

- Interactive data table with powerful search functionality
- Real-time data editing capabilities directly within the dashboard
- Instant database updates for seamless data management
- Responsive design ensuring optimal viewing across various devices and screen sizes
- User-friendly interface for easy navigation and data manipulation

## Prerequisites

Before you begin, ensure you have met the following requirements:

- Python 3.7+
- MySQL Server
- pip (Python package manager)

## Installation

1. Clone the repository:
   ```
   git clone https://github.com/your-username/kcs-dashboard.git
   cd kcs-dashboard
   ```

2. Install the required Python packages:
   ```
   pip install -r requirements.txt
   ```

3. Set up your MySQL database:
   - Create a database named `SF2`
   - Create a table named `Atrain2` with the following columns:
     - BEDTC (primary key)
     - POH_DATE
     - IC_DATE
     - TI_DATE
     - IA_DATE
     - WASHING_DATE
     - MOPPING_DATE

4. Update the database connection details in `report.py`:
   ```python
   db = mysql.connector.connect(
       host="your_host",
       user="your_username",
       password="your_password",
       database="SF2"
   )
   ```

## Usage

To run the dashboard:

```
python report.py
```

Then open a web browser and navigate to `http://127.0.0.1:8050/`

## Contributing

Contributions to the KCS Dashboard are welcome. Please follow these steps:

1. Fork the repository
2. Create a new branch: `git checkout -b <branch_name>`
3. Make your changes and commit them: `git commit -m '<commit_message>'`
4. Push to the original branch: `git push origin <project_name>/<location>`
5. Create the pull request

Alternatively, see the GitHub documentation on [creating a pull request](https://help.github.com/articles/creating-a-pull-request/).

## License

This project uses the following license: [MIT License](LICENSE).

## Contact

If you want to contact me, you can reach me at `<adityachandgaonkar30@gmail.com>`.
