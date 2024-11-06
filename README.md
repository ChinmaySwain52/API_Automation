data-driven-framework/
│
├── config/              
│   └── config.yml             # Stores configurations like environment URLs, DB credentials, etc.
│
├── data/                      
│   ├── test_data.csv          # CSV file containing test data for data-driven tests
│   ├── test_data.xlsx         # Excel file containing test data
│   ├── test_data.json         # JSON file with complex test data structures for API testing
│   └── database.sql           # SQL queries or scripts to prepare database with test data
│
├── src/                       
│   ├── test_scripts/         
│   │   ├── test_login.py      # Example: Login test case
│   │   ├── test_checkout.py   # Example: Checkout test case
│   │   └── ...                # Additional test scripts
│   │
│   ├── data_providers/       
│   │   ├── csv_data_provider.py   # Module to read data from CSV
│   │   ├── excel_data_provider.py # Module to read data from Excel
│   │   ├── json_data_provider.py  # Module to read data from JSON
│   │   └── db_data_provider.py    # Module to read data from a database
│   │
│   ├── utilities/              
│   │   ├── logger.py           # Custom logging functionality
│   │   ├── config_reader.py    # Reads config file
│   │   ├── assert_helper.py    # Custom assertion methods
│   │   └── ...                 # Additional utilities
│   │
│   ├── reports/                
│   │   ├── execution_report.html  # Generated HTML report after test run
│   │   └── screenshots/          # Screenshots of failed tests
│   │
│   └── logs/                    
│       └── test_execution.log   # Log file capturing execution details
│
├── test_runner/                
│   ├── pytest.ini               # Pytest configuration (if using pytest)
│   ├── testng.xml               # TestNG XML (if using Java TestNG)
│   └── run_tests.py             # Main script to trigger tests
│
└── README.md                    # Documentation