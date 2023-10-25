[![Pylint](https://github.com/MaineDSA/MembershipDashboard/actions/workflows/pylint.yml/badge.svg?branch=main)](https://github.com/MaineDSA/MembershipDashboard/actions/workflows/pylint.yml)

# Membership Dashboard

Herein lies a Python script that builds a dashboard to analyze membership lists.
It uses the Dash framework for creating web-based data visualizations.

## Getting Started

To run this code, you'll need to have Python 3.9, 3.10, or 3.11 installed on your machine. You'll also need to install the required packages by running the following command from inside the project folder:

```shell
python3 -m pip install -r requirements.txt
```

## Usage

1. Clone the repository and navigate to the project folder.
2. Open a terminal and run the following command to start the dashboard:

```shell
python3 -m membership_dashboard
```

3. Open your browser and go to `http://localhost:8050` to view the dashboard.

## Features

The dashboard provides the following features:

- Dropdown menus in sidebar to select an active membership list and another to compare against.
- Timeline graph showing long-term trends across all loaded lists. Choose what is shown by selecting columns from the dropdown list.
- List table displaying the active membership list with the option to export a CSV. If a compare list is selected, only the rows that changed are shown.
- Metrics showing the number of constitutional members, members in good standing, expiring members, and lapsed members.
- Graphs displaying membership counts, dues, union membership, length of membership, and racial demographics.
- Standardizes some important membership list metrics across variances in membership list formatting going back to at least Jan 2020.

## Notes

- The membership lists should be in the form of zipped CSV files.
- The code assumes that the membership lists are located in the `maine_membership_list` folder.
- The membership lists should follow a specific naming convention: `maine_membership_list_<YYYYMMDD>.zip` containing a single csv file called `maine_membership_list.csv`.
- To change this file name to match your chapter, look at the top of the [scan_membership_lists.py](scan_membership_lists.py) file and change the string ```MEMB_LIST_NAME```.

Feel free to explore the code and modify it according to your needs!
