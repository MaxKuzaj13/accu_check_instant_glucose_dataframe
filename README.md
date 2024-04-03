# Glucose Level Summary Generator for Accu-check Instant 

This script is designed to generate a summary of glucose levels from a CSV file exported from an Accu-Check instant glucose meter. The summary includes categorization of glucose levels into different time periods such as fasting, after breakfast, after lunch, and after dinner.

## Requirements
- Python 3
- pandas library
- matplotlib and openpyxl

## Usage
1. Clone the repository or download the script.
2. Ensure you have Python 3 installed on your system.
3. Install the required dependencies using pip: pip install -r requirements.txt
4. Place your CSV file containing glucose level data in the same directory as the script.
5. Modify the script parameters according to your requirements:
    - `start_reports`: Specify the date from which you want to start the reports.
    - `language_choice`: Choose the language for the report labels ('ENG' for English or 'POL' for Polish).
6. Run the line by line or use Run all in Visual Studio Code or other using python notebooks (ipynb) like Jupyter Notebook/JupyterLab, Databricks, Google Colab... 
7. The script will generate a CSV file containing the summarized glucose levels and also export a styled HTML and Excel file.

## Notes
- The script assumes specific time ranges for categorizing glucose levels after breakfast, lunch, and dinner.
- It categorizes glucose levels based on the following labels: fasting, after breakfast, after lunch, and after dinner.
- The script uses pandas to read, manipulate, and summarize the data.

Feel free to modify the script according to your specific requirements or data format.

<div>
    <h2>This is an HTML section</h2>
    <style type="text/css">
#T_6576c th {
  text-align: center;
}
#T_6576c_row0_col0, #T_6576c_row11_col1, #T_6576c_row37_col0, #T_6576c_row41_col0, #T_6576c_row44_col0, #T_6576c_row52_col0, #T_6576c_row64_col0, #T_6576c_row77_col0, #T_6576c_row93_col3, #T_6576c_row107_col0, #T_6576c_row108_col0 {
  color: black;
  border-color: white;
  background-color: #eeeec9;
  color: #000000;
}
#T_6576c_row0_col1, #T_6576c_row25_col0, #T_6576c_row83_col1, #T_6576c_row83_col2, #T_6576c_row99_col0, #T_6576c_row110_col1, #T_6576c_row115_col0 {
  color: black;
  border-color: white;
  background-color: #e7e6b2;
  color: #000000;
}
#T_6576c_row0_col2, #T_6576c_row22_col2, #T_6576c_row23_col0, #T_6576c_row26_col0, #T_6576c_row27_col2, #T_6576c_row88_col0 {
  color: black;
  border-color: white;
  background-color: #eaeab9;
  color: #000000;
}
#T_6576c_row0_col3, #T_6576c_row2_col0, #T_6576c_row12_col0, #T_6576c_row19_col0, #T_6576c_row20_col0, #T_6576c_row24_col0, #T_6576c_row73_col0 {
  color: black;
  border-color: white;
  background-color: #ddcda5;
  color: #000000;
}
#T_6576c_row1_col0, #T_6576c_row36_col0, #T_6576c_row60_col2, #T_6576c_row66_col0, #T_6576c_row110_col0 {
  color: black;
  border-color: white;
  background-color: #ebebbe;
  color: #000000;
}
#T_6576c_row1_col1, #T_6576c_row1_col2, #T_6576c_row1_col3, #T_6576c_row2_col1, #T_6576c_row2_col2, #T_6576c_row2_col3, #T_6576c_row3_col1, #T_6576c_row3_col2, #T_6576c_row3_col3, #T_6576c_row4_col1, #T_6576c_row4_col2, #T_6576c_row4_col3, #T_6576c_row6_col1, #T_6576c_row6_col2, #T_6576c_row6_col3, #T_6576c_row8_col1, #T_6576c_row8_col2, #T_6576c_row8_col3, #T_6576c_row9_col1, #T_6576c_row9_col2, #T_6576c_row9_col3, #T_6576c_row10_col1, #T_6576c_row10_col2, #T_6576c_row10_col3, #T_6576c_row12_col1, #T_6576c_row12_col2, #T_6576c_row12_col3, #T_6576c_row13_col1, #T_6576c_row13_col2, #T_6576c_row13_col3, #T_6576c_row14_col1, #T_6576c_row14_col2, #T_6576c_row14_col3, #T_6576c_row15_col1, #T_6576c_row15_col2, #T_6576c_row15_col3, #T_6576c_row16_col1, #T_6576c_row16_col2, #T_6576c_row16_col3, #T_6576c_row18_col1, #T_6576c_row18_col2, #T_6576c_row18_col3, #T_6576c_row19_col1, #T_6576c_row19_col2, #T_6576c_row19_col3, #T_6576c_row20_col1, #T_6576c_row20_col2, #T_6576c_row20_col3, #T_6576c_row21_col1, #T_6576c_row21_col2, #T_6576c_row21_col3, #T_6576c_row23_col1, #T_6576c_row23_col2, #T_6576c_row23_col3, #T_6576c_row24_col1, #T_6576c_row24_col2, #T_6576c_row24_col3, #T_6576c_row25_col1, #T_6576c_row25_col2, #T_6576c_row25_col3, #T_6576c_row26_col1, #T_6576c_row26_col2, #T_6576c_row26_col3, #T_6576c_row28_col1, #T_6576c_row28_col2, #T_6576c_row28_col3, #T_6576c_row29_col1, #T_6576c_row29_col2, #T_6576c_row29_col3, #T_6576c_row30_col1, #T_6576c_row30_col2, #T_6576c_row30_col3, #T_6576c_row31_col1, #T_6576c_row31_col2, #T_6576c_row31_col3, #T_6576c_row32_col1, #T_6576c_row32_col2, #T_6576c_row32_col3, #T_6576c_row33_col1, #T_6576c_row33_col2, #T_6576c_row33_col3, #T_6576c_row34_col1, #T_6576c_row34_col2, #T_6576c_row34_col3, #T_6576c_row36_col1, #T_6576c_row36_col2, #T_6576c_row36_col3, #T_6576c_row37_col2, #T_6576c_row38_col1, #T_6576c_row38_col2, #T_6576c_row38_col3, #T_6576c_row39_col1, #T_6576c_row39_col2, #T_6576c_row39_col3, #T_6576c_row40_col1, #T_6576c_row40_col2, #T_6576c_row40_col3, #T_6576c_row41_col1, #T_6576c_row41_col2, #T_6576c_row41_col3, #T_6576c_row42_col1, #T_6576c_row42_col2, #T_6576c_row42_col3, #T_6576c_row44_col1, #T_6576c_row44_col2, #T_6576c_row44_col3, #T_6576c_row45_col1, #T_6576c_row45_col2, #T_6576c_row45_col3, #T_6576c_row46_col1, #T_6576c_row46_col2, #T_6576c_row46_col3, #T_6576c_row47_col1, #T_6576c_row47_col2, #T_6576c_row47_col3, #T_6576c_row48_col1, #T_6576c_row48_col2, #T_6576c_row48_col3, #T_6576c_row49_col1, #T_6576c_row49_col2, #T_6576c_row49_col3, #T_6576c_row50_col1, #T_6576c_row50_col2, #T_6576c_row50_col3, #T_6576c_row52_col1, #T_6576c_row52_col2, #T_6576c_row52_col3, #T_6576c_row53_col1, #T_6576c_row53_col2, #T_6576c_row53_col3, #T_6576c_row54_col1, #T_6576c_row54_col2, #T_6576c_row54_col3, #T_6576c_row55_col1, #T_6576c_row55_col2, #T_6576c_row55_col3, #T_6576c_row56_col1, #T_6576c_row56_col2, #T_6576c_row56_col3, #T_6576c_row58_col1, #T_6576c_row58_col2, #T_6576c_row58_col3, #T_6576c_row59_col1, #T_6576c_row59_col2, #T_6576c_row59_col3, #T_6576c_row61_col1, #T_6576c_row61_col2, #T_6576c_row61_col3, #T_6576c_row62_col1, #T_6576c_row62_col2, #T_6576c_row62_col3, #T_6576c_row63_col1, #T_6576c_row63_col2, #T_6576c_row63_col3, #T_6576c_row65_col1, #T_6576c_row65_col2, #T_6576c_row65_col3, #T_6576c_row66_col1, #T_6576c_row66_col2, #T_6576c_row66_col3, #T_6576c_row68_col1, #T_6576c_row68_col2, #T_6576c_row68_col3, #T_6576c_row69_col1, #T_6576c_row69_col2, #T_6576c_row69_col3, #T_6576c_row70_col1, #T_6576c_row70_col2, #T_6576c_row70_col3, #T_6576c_row71_col1, #T_6576c_row71_col2, #T_6576c_row71_col3, #T_6576c_row72_col1, #T_6576c_row72_col2, #T_6576c_row72_col3, #T_6576c_row73_col1, #T_6576c_row73_col2, #T_6576c_row73_col3, #T_6576c_row74_col1, #T_6576c_row74_col2, #T_6576c_row74_col3, #T_6576c_row75_col1, #T_6576c_row75_col2, #T_6576c_row75_col3, #T_6576c_row77_col1, #T_6576c_row77_col2, #T_6576c_row77_col3, #T_6576c_row78_col1, #T_6576c_row78_col2, #T_6576c_row78_col3, #T_6576c_row79_col1, #T_6576c_row79_col2, #T_6576c_row79_col3, #T_6576c_row80_col1, #T_6576c_row80_col2, #T_6576c_row80_col3, #T_6576c_row81_col1, #T_6576c_row81_col2, #T_6576c_row81_col3, #T_6576c_row82_col1, #T_6576c_row82_col2, #T_6576c_row82_col3, #T_6576c_row84_col1, #T_6576c_row84_col2, #T_6576c_row84_col3, #T_6576c_row85_col1, #T_6576c_row85_col2, #T_6576c_row85_col3, #T_6576c_row86_col1, #T_6576c_row86_col2, #T_6576c_row86_col3, #T_6576c_row87_col1, #T_6576c_row87_col2, #T_6576c_row88_col1, #T_6576c_row88_col2, #T_6576c_row88_col3, #T_6576c_row89_col1, #T_6576c_row89_col2, #T_6576c_row89_col3, #T_6576c_row90_col1, #T_6576c_row90_col2, #T_6576c_row90_col3, #T_6576c_row91_col1, #T_6576c_row91_col2, #T_6576c_row91_col3, #T_6576c_row92_col1, #T_6576c_row92_col2, #T_6576c_row92_col3, #T_6576c_row94_col1, #T_6576c_row94_col2, #T_6576c_row94_col3, #T_6576c_row95_col1, #T_6576c_row95_col2, #T_6576c_row95_col3, #T_6576c_row96_col1, #T_6576c_row96_col2, #T_6576c_row96_col3, #T_6576c_row97_col1, #T_6576c_row97_col2, #T_6576c_row97_col3, #T_6576c_row98_col1, #T_6576c_row98_col2, #T_6576c_row98_col3, #T_6576c_row99_col1, #T_6576c_row99_col2, #T_6576c_row99_col3, #T_6576c_row100_col1, #T_6576c_row100_col2, #T_6576c_row100_col3, #T_6576c_row101_col1, #T_6576c_row101_col2, #T_6576c_row101_col3, #T_6576c_row102_col1, #T_6576c_row102_col2, #T_6576c_row102_col3, #T_6576c_row104_col1, #T_6576c_row104_col2, #T_6576c_row104_col3, #T_6576c_row105_col1, #T_6576c_row105_col2, #T_6576c_row105_col3, #T_6576c_row106_col1, #T_6576c_row106_col2, #T_6576c_row106_col3, #T_6576c_row107_col1, #T_6576c_row107_col2, #T_6576c_row107_col3, #T_6576c_row108_col1, #T_6576c_row108_col2, #T_6576c_row108_col3, #T_6576c_row109_col1, #T_6576c_row109_col2, #T_6576c_row109_col3, #T_6576c_row111_col1, #T_6576c_row111_col2, #T_6576c_row111_col3, #T_6576c_row112_col1, #T_6576c_row112_col2, #T_6576c_row112_col3, #T_6576c_row113_col1, #T_6576c_row113_col2, #T_6576c_row113_col3, #T_6576c_row114_col1, #T_6576c_row114_col2, #T_6576c_row114_col3, #T_6576c_row115_col1, #T_6576c_row115_col2, #T_6576c_row115_col3 {
  color: black;
  border-color: white;
  background-color: #000000;
  color: #f1f1f1;
}
#T_6576c_row3_col0, #T_6576c_row5_col3, #T_6576c_row78_col0, #T_6576c_row86_col0, #T_6576c_row87_col3, #T_6576c_row103_col2 {
  color: black;
  border-color: white;
  background-color: #f3f3db;
  color: #000000;
}
#T_6576c_row4_col0, #T_6576c_row93_col2, #T_6576c_row96_col0 {
  color: black;
  border-color: white;
  background-color: #ffffff;
  color: #000000;
}
#T_6576c_row5_col0, #T_6576c_row64_col1, #T_6576c_row91_col0 {
  color: black;
  border-color: white;
  background-color: #f1f1d1;
  color: #000000;
}
#T_6576c_row5_col1, #T_6576c_row6_col0, #T_6576c_row22_col1, #T_6576c_row57_col2, #T_6576c_row102_col0, #T_6576c_row104_col0 {
  color: black;
  border-color: white;
  background-color: #ededc4;
  color: #000000;
}
#T_6576c_row5_col2, #T_6576c_row60_col3 {
  color: black;
  border-color: white;
  background-color: #d9c29f;
  color: #000000;
}
#T_6576c_row7_col0, #T_6576c_row21_col0 {
  color: black;
  border-color: white;
  background-color: #f2f2d6;
  color: #000000;
}
#T_6576c_row7_col1, #T_6576c_row27_col0, #T_6576c_row27_col1, #T_6576c_row35_col0, #T_6576c_row42_col0, #T_6576c_row64_col2, #T_6576c_row83_col0, #T_6576c_row97_col0, #T_6576c_row101_col0 {
  color: black;
  border-color: white;
  background-color: #e6e2b0;
  color: #000000;
}
#T_6576c_row7_col2, #T_6576c_row67_col0, #T_6576c_row68_col0 {
  color: black;
  border-color: white;
  background-color: #d4b699;
  color: #000000;
}
#T_6576c_row7_col3 {
  color: black;
  border-color: white;
  background-color: #cb9b8b;
  color: #f1f1f1;
}
#T_6576c_row8_col0, #T_6576c_row17_col0, #T_6576c_row28_col0, #T_6576c_row38_col0, #T_6576c_row53_col0, #T_6576c_row55_col0, #T_6576c_row61_col0, #T_6576c_row67_col1, #T_6576c_row67_col2, #T_6576c_row79_col0, #T_6576c_row85_col0 {
  color: black;
  border-color: white;
  background-color: #e1d8aa;
  color: #000000;
}
#T_6576c_row9_col0, #T_6576c_row29_col0, #T_6576c_row50_col0, #T_6576c_row51_col1, #T_6576c_row51_col2, #T_6576c_row54_col0, #T_6576c_row76_col1, #T_6576c_row100_col0, #T_6576c_row110_col2 {
  color: black;
  border-color: white;
  background-color: #e9e9b5;
  color: #000000;
}
#T_6576c_row10_col0, #T_6576c_row17_col1, #T_6576c_row32_col0, #T_6576c_row33_col0, #T_6576c_row72_col0 {
  color: black;
  border-color: white;
  background-color: #dac5a1;
  color: #000000;
}
#T_6576c_row11_col0, #T_6576c_row16_col0, #T_6576c_row103_col1 {
  color: black;
  border-color: white;
  background-color: #f5f5df;
  color: #000000;
}
#T_6576c_row11_col2, #T_6576c_row43_col3, #T_6576c_row69_col0, #T_6576c_row89_col0, #T_6576c_row103_col0 {
  color: black;
  border-color: white;
  background-color: #dcc9a3;
  color: #000000;
}
#T_6576c_row11_col3, #T_6576c_row35_col1, #T_6576c_row46_col0, #T_6576c_row60_col1, #T_6576c_row71_col0, #T_6576c_row76_col2, #T_6576c_row81_col0, #T_6576c_row83_col3, #T_6576c_row105_col0, #T_6576c_row113_col0 {
  color: black;
  border-color: white;
  background-color: #e4dfae;
  color: #000000;
}
#T_6576c_row13_col0, #T_6576c_row14_col0, #T_6576c_row35_col2, #T_6576c_row43_col1, #T_6576c_row43_col2, #T_6576c_row47_col0, #T_6576c_row48_col0, #T_6576c_row58_col0, #T_6576c_row75_col0, #T_6576c_row80_col0, #T_6576c_row84_col0 {
  color: black;
  border-color: white;
  background-color: #e0d5a9;
  color: #000000;
}
#T_6576c_row15_col0, #T_6576c_row34_col0, #T_6576c_row37_col1, #T_6576c_row57_col0, #T_6576c_row60_col0, #T_6576c_row87_col0, #T_6576c_row90_col0, #T_6576c_row92_col0, #T_6576c_row93_col1, #T_6576c_row106_col0, #T_6576c_row114_col0 {
  color: black;
  border-color: white;
  background-color: #dfd1a7;
  color: #000000;
}
#T_6576c_row17_col2 {
  color: black;
  border-color: white;
  background-color: #cca08e;
  color: #f1f1f1;
}
#T_6576c_row17_col3 {
  color: black;
  border-color: white;
  background-color: #c68c84;
  color: #f1f1f1;
}
#T_6576c_row18_col0, #T_6576c_row31_col0, #T_6576c_row39_col0, #T_6576c_row43_col0, #T_6576c_row49_col0, #T_6576c_row56_col0, #T_6576c_row57_col1, #T_6576c_row59_col0, #T_6576c_row62_col0, #T_6576c_row64_col3, #T_6576c_row65_col0, #T_6576c_row82_col0, #T_6576c_row95_col0 {
  color: black;
  border-color: white;
  background-color: #e3dbac;
  color: #000000;
}
#T_6576c_row22_col0 {
  color: black;
  border-color: white;
  background-color: #f9f9eb;
  color: #000000;
}
#T_6576c_row22_col3 {
  color: black;
  border-color: white;
  background-color: #935f5f;
  color: #f1f1f1;
}
#T_6576c_row27_col3, #T_6576c_row35_col3, #T_6576c_row94_col0 {
  color: black;
  border-color: white;
  background-color: #d6ba9b;
  color: #000000;
}
#T_6576c_row30_col0, #T_6576c_row51_col0 {
  color: black;
  border-color: white;
  background-color: #f0f0ce;
  color: #000000;
}
#T_6576c_row37_col3 {
  color: black;
  border-color: white;
  background-color: #cea590;
  color: #000000;
}
#T_6576c_row40_col0, #T_6576c_row63_col0 {
  color: black;
  border-color: white;
  background-color: #f8f8e8;
  color: #000000;
}
#T_6576c_row45_col0 {
  color: black;
  border-color: white;
  background-color: #f6f6e4;
  color: #000000;
}
#T_6576c_row51_col3, #T_6576c_row70_col0, #T_6576c_row74_col0, #T_6576c_row109_col0 {
  color: black;
  border-color: white;
  background-color: #d7be9d;
  color: #000000;
}
#T_6576c_row57_col3, #T_6576c_row76_col3 {
  color: black;
  border-color: white;
  background-color: #c99689;
  color: #f1f1f1;
}
#T_6576c_row67_col3 {
  color: black;
  border-color: white;
  background-color: #bb7a7a;
  color: #f1f1f1;
}
#T_6576c_row76_col0 {
  color: black;
  border-color: white;
  background-color: #fafaf0;
  color: #000000;
}
#T_6576c_row93_col0 {
  color: black;
  border-color: white;
  background-color: #d1ad94;
  color: #000000;
}
#T_6576c_row98_col0 {
  color: black;
  border-color: white;
  background-color: #a66c6c;
  color: #f1f1f1;
}
#T_6576c_row103_col3 {
  color: black;
  border-color: white;
  background-color: #7e5050;
  color: #f1f1f1;
}
#T_6576c_row110_col3 {
  color: black;
  border-color: white;
  background-color: #1e0000;
  color: #f1f1f1;
}
#T_6576c_row111_col0 {
  color: black;
  border-color: white;
  background-color: #c79186;
  color: #f1f1f1;
}
#T_6576c_row112_col0 {
  color: black;
  border-color: white;
  background-color: #c48782;
  color: #f1f1f1;
}
</style>
<table id="T_6576c">
  <caption>Zbiorcze zestawienie poziomu cukru od dnia 2023-10-10.csv</caption>
  <thead>
    <tr>
      <th class="index_name level0" >label</th>
      <th id="T_6576c_level0_col0" class="col_heading level0 col0" >Nadczo</th>
      <th id="T_6576c_level0_col1" class="col_heading level0 col1" >Po śniadaniu</th>
      <th id="T_6576c_level0_col2" class="col_heading level0 col2" >Po obiedzie</th>
      <th id="T_6576c_level0_col3" class="col_heading level0 col3" >Po kolacji</th>
    </tr>
    <tr>
      <th class="index_name level0" >date</th>
      <th class="blank col0" >&nbsp;</th>
      <th class="blank col1" >&nbsp;</th>
      <th class="blank col2" >&nbsp;</th>
      <th class="blank col3" >&nbsp;</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th id="T_6576c_level0_row0" class="row_heading level0 row0" >2023-10-10</th>
      <td id="T_6576c_row0_col0" class="data row0 col0" >96</td>
      <td id="T_6576c_row0_col1" class="data row0 col1" >101</td>
      <td id="T_6576c_row0_col2" class="data row0 col2" >99</td>
      <td id="T_6576c_row0_col3" class="data row0 col3" >108</td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row1" class="row_heading level0 row1" >2023-10-11</th>
      <td id="T_6576c_row1_col0" class="data row1 col0" >98</td>
      <td id="T_6576c_row1_col1" class="data row1 col1" ></td>
      <td id="T_6576c_row1_col2" class="data row1 col2" ></td>
      <td id="T_6576c_row1_col3" class="data row1 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row2" class="row_heading level0 row2" >2023-10-13</th>
      <td id="T_6576c_row2_col0" class="data row2 col0" >108</td>
      <td id="T_6576c_row2_col1" class="data row2 col1" ></td>
      <td id="T_6576c_row2_col2" class="data row2 col2" ></td>
      <td id="T_6576c_row2_col3" class="data row2 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row3" class="row_heading level0 row3" >2023-10-15</th>
      <td id="T_6576c_row3_col0" class="data row3 col0" >92</td>
      <td id="T_6576c_row3_col1" class="data row3 col1" ></td>
      <td id="T_6576c_row3_col2" class="data row3 col2" ></td>
      <td id="T_6576c_row3_col3" class="data row3 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row4" class="row_heading level0 row4" >2023-10-16</th>
      <td id="T_6576c_row4_col0" class="data row4 col0" >83</td>
      <td id="T_6576c_row4_col1" class="data row4 col1" ></td>
      <td id="T_6576c_row4_col2" class="data row4 col2" ></td>
      <td id="T_6576c_row4_col3" class="data row4 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row5" class="row_heading level0 row5" >2023-10-19</th>
      <td id="T_6576c_row5_col0" class="data row5 col0" >94</td>
      <td id="T_6576c_row5_col1" class="data row5 col1" >97</td>
      <td id="T_6576c_row5_col2" class="data row5 col2" >111</td>
      <td id="T_6576c_row5_col3" class="data row5 col3" >92</td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row6" class="row_heading level0 row6" >2023-10-20</th>
      <td id="T_6576c_row6_col0" class="data row6 col0" >97</td>
      <td id="T_6576c_row6_col1" class="data row6 col1" ></td>
      <td id="T_6576c_row6_col2" class="data row6 col2" ></td>
      <td id="T_6576c_row6_col3" class="data row6 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row7" class="row_heading level0 row7" >2023-10-23</th>
      <td id="T_6576c_row7_col0" class="data row7 col0" >93</td>
      <td id="T_6576c_row7_col1" class="data row7 col1" >102</td>
      <td id="T_6576c_row7_col2" class="data row7 col2" >114</td>
      <td id="T_6576c_row7_col3" class="data row7 col3" >120</td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row8" class="row_heading level0 row8" >2023-10-24</th>
      <td id="T_6576c_row8_col0" class="data row8 col0" >105</td>
      <td id="T_6576c_row8_col1" class="data row8 col1" ></td>
      <td id="T_6576c_row8_col2" class="data row8 col2" ></td>
      <td id="T_6576c_row8_col3" class="data row8 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row9" class="row_heading level0 row9" >2023-10-25</th>
      <td id="T_6576c_row9_col0" class="data row9 col0" >100</td>
      <td id="T_6576c_row9_col1" class="data row9 col1" ></td>
      <td id="T_6576c_row9_col2" class="data row9 col2" ></td>
      <td id="T_6576c_row9_col3" class="data row9 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row10" class="row_heading level0 row10" >2023-10-27</th>
      <td id="T_6576c_row10_col0" class="data row10 col0" >110</td>
      <td id="T_6576c_row10_col1" class="data row10 col1" ></td>
      <td id="T_6576c_row10_col2" class="data row10 col2" ></td>
      <td id="T_6576c_row10_col3" class="data row10 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row11" class="row_heading level0 row11" >2023-10-30</th>
      <td id="T_6576c_row11_col0" class="data row11 col0" >91</td>
      <td id="T_6576c_row11_col1" class="data row11 col1" >96</td>
      <td id="T_6576c_row11_col2" class="data row11 col2" >109</td>
      <td id="T_6576c_row11_col3" class="data row11 col3" >103</td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row12" class="row_heading level0 row12" >2023-10-31</th>
      <td id="T_6576c_row12_col0" class="data row12 col0" >108</td>
      <td id="T_6576c_row12_col1" class="data row12 col1" ></td>
      <td id="T_6576c_row12_col2" class="data row12 col2" ></td>
      <td id="T_6576c_row12_col3" class="data row12 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row13" class="row_heading level0 row13" >2023-11-01</th>
      <td id="T_6576c_row13_col0" class="data row13 col0" >106</td>
      <td id="T_6576c_row13_col1" class="data row13 col1" ></td>
      <td id="T_6576c_row13_col2" class="data row13 col2" ></td>
      <td id="T_6576c_row13_col3" class="data row13 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row14" class="row_heading level0 row14" >2023-11-02</th>
      <td id="T_6576c_row14_col0" class="data row14 col0" >106</td>
      <td id="T_6576c_row14_col1" class="data row14 col1" ></td>
      <td id="T_6576c_row14_col2" class="data row14 col2" ></td>
      <td id="T_6576c_row14_col3" class="data row14 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row15" class="row_heading level0 row15" >2023-11-03</th>
      <td id="T_6576c_row15_col0" class="data row15 col0" >107</td>
      <td id="T_6576c_row15_col1" class="data row15 col1" ></td>
      <td id="T_6576c_row15_col2" class="data row15 col2" ></td>
      <td id="T_6576c_row15_col3" class="data row15 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row16" class="row_heading level0 row16" >2023-11-04</th>
      <td id="T_6576c_row16_col0" class="data row16 col0" >91</td>
      <td id="T_6576c_row16_col1" class="data row16 col1" ></td>
      <td id="T_6576c_row16_col2" class="data row16 col2" ></td>
      <td id="T_6576c_row16_col3" class="data row16 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row17" class="row_heading level0 row17" >2023-11-06</th>
      <td id="T_6576c_row17_col0" class="data row17 col0" >105</td>
      <td id="T_6576c_row17_col1" class="data row17 col1" >110</td>
      <td id="T_6576c_row17_col2" class="data row17 col2" >119</td>
      <td id="T_6576c_row17_col3" class="data row17 col3" >123</td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row18" class="row_heading level0 row18" >2023-11-07</th>
      <td id="T_6576c_row18_col0" class="data row18 col0" >104</td>
      <td id="T_6576c_row18_col1" class="data row18 col1" ></td>
      <td id="T_6576c_row18_col2" class="data row18 col2" ></td>
      <td id="T_6576c_row18_col3" class="data row18 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row19" class="row_heading level0 row19" >2023-11-08</th>
      <td id="T_6576c_row19_col0" class="data row19 col0" >108</td>
      <td id="T_6576c_row19_col1" class="data row19 col1" ></td>
      <td id="T_6576c_row19_col2" class="data row19 col2" ></td>
      <td id="T_6576c_row19_col3" class="data row19 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row20" class="row_heading level0 row20" >2023-11-10</th>
      <td id="T_6576c_row20_col0" class="data row20 col0" >108</td>
      <td id="T_6576c_row20_col1" class="data row20 col1" ></td>
      <td id="T_6576c_row20_col2" class="data row20 col2" ></td>
      <td id="T_6576c_row20_col3" class="data row20 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row21" class="row_heading level0 row21" >2023-11-11</th>
      <td id="T_6576c_row21_col0" class="data row21 col0" >93</td>
      <td id="T_6576c_row21_col1" class="data row21 col1" ></td>
      <td id="T_6576c_row21_col2" class="data row21 col2" ></td>
      <td id="T_6576c_row21_col3" class="data row21 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row22" class="row_heading level0 row22" >2023-11-13</th>
      <td id="T_6576c_row22_col0" class="data row22 col0" >88</td>
      <td id="T_6576c_row22_col1" class="data row22 col1" >97</td>
      <td id="T_6576c_row22_col2" class="data row22 col2" >99</td>
      <td id="T_6576c_row22_col3" class="data row22 col3" >136</td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row23" class="row_heading level0 row23" >2023-11-14</th>
      <td id="T_6576c_row23_col0" class="data row23 col0" >99</td>
      <td id="T_6576c_row23_col1" class="data row23 col1" ></td>
      <td id="T_6576c_row23_col2" class="data row23 col2" ></td>
      <td id="T_6576c_row23_col3" class="data row23 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row24" class="row_heading level0 row24" >2023-11-16</th>
      <td id="T_6576c_row24_col0" class="data row24 col0" >108</td>
      <td id="T_6576c_row24_col1" class="data row24 col1" ></td>
      <td id="T_6576c_row24_col2" class="data row24 col2" ></td>
      <td id="T_6576c_row24_col3" class="data row24 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row25" class="row_heading level0 row25" >2023-11-17</th>
      <td id="T_6576c_row25_col0" class="data row25 col0" >101</td>
      <td id="T_6576c_row25_col1" class="data row25 col1" ></td>
      <td id="T_6576c_row25_col2" class="data row25 col2" ></td>
      <td id="T_6576c_row25_col3" class="data row25 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row26" class="row_heading level0 row26" >2023-11-19</th>
      <td id="T_6576c_row26_col0" class="data row26 col0" >99</td>
      <td id="T_6576c_row26_col1" class="data row26 col1" ></td>
      <td id="T_6576c_row26_col2" class="data row26 col2" ></td>
      <td id="T_6576c_row26_col3" class="data row26 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row27" class="row_heading level0 row27" >2023-11-20</th>
      <td id="T_6576c_row27_col0" class="data row27 col0" >102</td>
      <td id="T_6576c_row27_col1" class="data row27 col1" >102</td>
      <td id="T_6576c_row27_col2" class="data row27 col2" >99</td>
      <td id="T_6576c_row27_col3" class="data row27 col3" >113</td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row28" class="row_heading level0 row28" >2023-11-21</th>
      <td id="T_6576c_row28_col0" class="data row28 col0" >105</td>
      <td id="T_6576c_row28_col1" class="data row28 col1" ></td>
      <td id="T_6576c_row28_col2" class="data row28 col2" ></td>
      <td id="T_6576c_row28_col3" class="data row28 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row29" class="row_heading level0 row29" >2023-11-22</th>
      <td id="T_6576c_row29_col0" class="data row29 col0" >100</td>
      <td id="T_6576c_row29_col1" class="data row29 col1" ></td>
      <td id="T_6576c_row29_col2" class="data row29 col2" ></td>
      <td id="T_6576c_row29_col3" class="data row29 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row30" class="row_heading level0 row30" >2023-11-23</th>
      <td id="T_6576c_row30_col0" class="data row30 col0" >95</td>
      <td id="T_6576c_row30_col1" class="data row30 col1" ></td>
      <td id="T_6576c_row30_col2" class="data row30 col2" ></td>
      <td id="T_6576c_row30_col3" class="data row30 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row31" class="row_heading level0 row31" >2023-11-24</th>
      <td id="T_6576c_row31_col0" class="data row31 col0" >104</td>
      <td id="T_6576c_row31_col1" class="data row31 col1" ></td>
      <td id="T_6576c_row31_col2" class="data row31 col2" ></td>
      <td id="T_6576c_row31_col3" class="data row31 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row32" class="row_heading level0 row32" >2023-11-27</th>
      <td id="T_6576c_row32_col0" class="data row32 col0" >110</td>
      <td id="T_6576c_row32_col1" class="data row32 col1" ></td>
      <td id="T_6576c_row32_col2" class="data row32 col2" ></td>
      <td id="T_6576c_row32_col3" class="data row32 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row33" class="row_heading level0 row33" >2023-11-28</th>
      <td id="T_6576c_row33_col0" class="data row33 col0" >110</td>
      <td id="T_6576c_row33_col1" class="data row33 col1" ></td>
      <td id="T_6576c_row33_col2" class="data row33 col2" ></td>
      <td id="T_6576c_row33_col3" class="data row33 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row34" class="row_heading level0 row34" >2023-11-29</th>
      <td id="T_6576c_row34_col0" class="data row34 col0" >107</td>
      <td id="T_6576c_row34_col1" class="data row34 col1" ></td>
      <td id="T_6576c_row34_col2" class="data row34 col2" ></td>
      <td id="T_6576c_row34_col3" class="data row34 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row35" class="row_heading level0 row35" >2023-11-30</th>
      <td id="T_6576c_row35_col0" class="data row35 col0" >102</td>
      <td id="T_6576c_row35_col1" class="data row35 col1" >103</td>
      <td id="T_6576c_row35_col2" class="data row35 col2" >106</td>
      <td id="T_6576c_row35_col3" class="data row35 col3" >113</td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row36" class="row_heading level0 row36" >2023-12-01</th>
      <td id="T_6576c_row36_col0" class="data row36 col0" >98</td>
      <td id="T_6576c_row36_col1" class="data row36 col1" ></td>
      <td id="T_6576c_row36_col2" class="data row36 col2" ></td>
      <td id="T_6576c_row36_col3" class="data row36 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row37" class="row_heading level0 row37" >2023-12-04</th>
      <td id="T_6576c_row37_col0" class="data row37 col0" >96</td>
      <td id="T_6576c_row37_col1" class="data row37 col1" >107</td>
      <td id="T_6576c_row37_col2" class="data row37 col2" ></td>
      <td id="T_6576c_row37_col3" class="data row37 col3" >118</td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row38" class="row_heading level0 row38" >2023-12-06</th>
      <td id="T_6576c_row38_col0" class="data row38 col0" >105</td>
      <td id="T_6576c_row38_col1" class="data row38 col1" ></td>
      <td id="T_6576c_row38_col2" class="data row38 col2" ></td>
      <td id="T_6576c_row38_col3" class="data row38 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row39" class="row_heading level0 row39" >2023-12-07</th>
      <td id="T_6576c_row39_col0" class="data row39 col0" >104</td>
      <td id="T_6576c_row39_col1" class="data row39 col1" ></td>
      <td id="T_6576c_row39_col2" class="data row39 col2" ></td>
      <td id="T_6576c_row39_col3" class="data row39 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row40" class="row_heading level0 row40" >2023-12-08</th>
      <td id="T_6576c_row40_col0" class="data row40 col0" >89</td>
      <td id="T_6576c_row40_col1" class="data row40 col1" ></td>
      <td id="T_6576c_row40_col2" class="data row40 col2" ></td>
      <td id="T_6576c_row40_col3" class="data row40 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row41" class="row_heading level0 row41" >2023-12-11</th>
      <td id="T_6576c_row41_col0" class="data row41 col0" >96</td>
      <td id="T_6576c_row41_col1" class="data row41 col1" ></td>
      <td id="T_6576c_row41_col2" class="data row41 col2" ></td>
      <td id="T_6576c_row41_col3" class="data row41 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row42" class="row_heading level0 row42" >2023-12-12</th>
      <td id="T_6576c_row42_col0" class="data row42 col0" >102</td>
      <td id="T_6576c_row42_col1" class="data row42 col1" ></td>
      <td id="T_6576c_row42_col2" class="data row42 col2" ></td>
      <td id="T_6576c_row42_col3" class="data row42 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row43" class="row_heading level0 row43" >2023-12-13</th>
      <td id="T_6576c_row43_col0" class="data row43 col0" >104</td>
      <td id="T_6576c_row43_col1" class="data row43 col1" >106</td>
      <td id="T_6576c_row43_col2" class="data row43 col2" >106</td>
      <td id="T_6576c_row43_col3" class="data row43 col3" >109</td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row44" class="row_heading level0 row44" >2023-12-14</th>
      <td id="T_6576c_row44_col0" class="data row44 col0" >96</td>
      <td id="T_6576c_row44_col1" class="data row44 col1" ></td>
      <td id="T_6576c_row44_col2" class="data row44 col2" ></td>
      <td id="T_6576c_row44_col3" class="data row44 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row45" class="row_heading level0 row45" >2023-12-17</th>
      <td id="T_6576c_row45_col0" class="data row45 col0" >90</td>
      <td id="T_6576c_row45_col1" class="data row45 col1" ></td>
      <td id="T_6576c_row45_col2" class="data row45 col2" ></td>
      <td id="T_6576c_row45_col3" class="data row45 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row46" class="row_heading level0 row46" >2023-12-20</th>
      <td id="T_6576c_row46_col0" class="data row46 col0" >103</td>
      <td id="T_6576c_row46_col1" class="data row46 col1" ></td>
      <td id="T_6576c_row46_col2" class="data row46 col2" ></td>
      <td id="T_6576c_row46_col3" class="data row46 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row47" class="row_heading level0 row47" >2023-12-22</th>
      <td id="T_6576c_row47_col0" class="data row47 col0" >106</td>
      <td id="T_6576c_row47_col1" class="data row47 col1" ></td>
      <td id="T_6576c_row47_col2" class="data row47 col2" ></td>
      <td id="T_6576c_row47_col3" class="data row47 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row48" class="row_heading level0 row48" >2023-12-23</th>
      <td id="T_6576c_row48_col0" class="data row48 col0" >106</td>
      <td id="T_6576c_row48_col1" class="data row48 col1" ></td>
      <td id="T_6576c_row48_col2" class="data row48 col2" ></td>
      <td id="T_6576c_row48_col3" class="data row48 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row49" class="row_heading level0 row49" >2023-12-25</th>
      <td id="T_6576c_row49_col0" class="data row49 col0" >104</td>
      <td id="T_6576c_row49_col1" class="data row49 col1" ></td>
      <td id="T_6576c_row49_col2" class="data row49 col2" ></td>
      <td id="T_6576c_row49_col3" class="data row49 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row50" class="row_heading level0 row50" >2023-12-27</th>
      <td id="T_6576c_row50_col0" class="data row50 col0" >100</td>
      <td id="T_6576c_row50_col1" class="data row50 col1" ></td>
      <td id="T_6576c_row50_col2" class="data row50 col2" ></td>
      <td id="T_6576c_row50_col3" class="data row50 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row51" class="row_heading level0 row51" >2023-12-28</th>
      <td id="T_6576c_row51_col0" class="data row51 col0" >95</td>
      <td id="T_6576c_row51_col1" class="data row51 col1" >100</td>
      <td id="T_6576c_row51_col2" class="data row51 col2" >100</td>
      <td id="T_6576c_row51_col3" class="data row51 col3" >112</td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row52" class="row_heading level0 row52" >2023-12-29</th>
      <td id="T_6576c_row52_col0" class="data row52 col0" >96</td>
      <td id="T_6576c_row52_col1" class="data row52 col1" ></td>
      <td id="T_6576c_row52_col2" class="data row52 col2" ></td>
      <td id="T_6576c_row52_col3" class="data row52 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row53" class="row_heading level0 row53" >2023-12-30</th>
      <td id="T_6576c_row53_col0" class="data row53 col0" >105</td>
      <td id="T_6576c_row53_col1" class="data row53 col1" ></td>
      <td id="T_6576c_row53_col2" class="data row53 col2" ></td>
      <td id="T_6576c_row53_col3" class="data row53 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row54" class="row_heading level0 row54" >2023-12-31</th>
      <td id="T_6576c_row54_col0" class="data row54 col0" >100</td>
      <td id="T_6576c_row54_col1" class="data row54 col1" ></td>
      <td id="T_6576c_row54_col2" class="data row54 col2" ></td>
      <td id="T_6576c_row54_col3" class="data row54 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row55" class="row_heading level0 row55" >2024-01-01</th>
      <td id="T_6576c_row55_col0" class="data row55 col0" >105</td>
      <td id="T_6576c_row55_col1" class="data row55 col1" ></td>
      <td id="T_6576c_row55_col2" class="data row55 col2" ></td>
      <td id="T_6576c_row55_col3" class="data row55 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row56" class="row_heading level0 row56" >2024-01-03</th>
      <td id="T_6576c_row56_col0" class="data row56 col0" >104</td>
      <td id="T_6576c_row56_col1" class="data row56 col1" ></td>
      <td id="T_6576c_row56_col2" class="data row56 col2" ></td>
      <td id="T_6576c_row56_col3" class="data row56 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row57" class="row_heading level0 row57" >2024-01-04</th>
      <td id="T_6576c_row57_col0" class="data row57 col0" >107</td>
      <td id="T_6576c_row57_col1" class="data row57 col1" >104</td>
      <td id="T_6576c_row57_col2" class="data row57 col2" >97</td>
      <td id="T_6576c_row57_col3" class="data row57 col3" >121</td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row58" class="row_heading level0 row58" >2024-01-08</th>
      <td id="T_6576c_row58_col0" class="data row58 col0" >106</td>
      <td id="T_6576c_row58_col1" class="data row58 col1" ></td>
      <td id="T_6576c_row58_col2" class="data row58 col2" ></td>
      <td id="T_6576c_row58_col3" class="data row58 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row59" class="row_heading level0 row59" >2024-01-09</th>
      <td id="T_6576c_row59_col0" class="data row59 col0" >104</td>
      <td id="T_6576c_row59_col1" class="data row59 col1" ></td>
      <td id="T_6576c_row59_col2" class="data row59 col2" ></td>
      <td id="T_6576c_row59_col3" class="data row59 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row60" class="row_heading level0 row60" >2024-01-10</th>
      <td id="T_6576c_row60_col0" class="data row60 col0" >107</td>
      <td id="T_6576c_row60_col1" class="data row60 col1" >103</td>
      <td id="T_6576c_row60_col2" class="data row60 col2" >98</td>
      <td id="T_6576c_row60_col3" class="data row60 col3" >111</td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row61" class="row_heading level0 row61" >2024-01-11</th>
      <td id="T_6576c_row61_col0" class="data row61 col0" >105</td>
      <td id="T_6576c_row61_col1" class="data row61 col1" ></td>
      <td id="T_6576c_row61_col2" class="data row61 col2" ></td>
      <td id="T_6576c_row61_col3" class="data row61 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row62" class="row_heading level0 row62" >2024-01-12</th>
      <td id="T_6576c_row62_col0" class="data row62 col0" >104</td>
      <td id="T_6576c_row62_col1" class="data row62 col1" ></td>
      <td id="T_6576c_row62_col2" class="data row62 col2" ></td>
      <td id="T_6576c_row62_col3" class="data row62 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row63" class="row_heading level0 row63" >2024-01-13</th>
      <td id="T_6576c_row63_col0" class="data row63 col0" >89</td>
      <td id="T_6576c_row63_col1" class="data row63 col1" ></td>
      <td id="T_6576c_row63_col2" class="data row63 col2" ></td>
      <td id="T_6576c_row63_col3" class="data row63 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row64" class="row_heading level0 row64" >2024-01-15</th>
      <td id="T_6576c_row64_col0" class="data row64 col0" >96</td>
      <td id="T_6576c_row64_col1" class="data row64 col1" >94</td>
      <td id="T_6576c_row64_col2" class="data row64 col2" >102</td>
      <td id="T_6576c_row64_col3" class="data row64 col3" >104</td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row65" class="row_heading level0 row65" >2024-01-16</th>
      <td id="T_6576c_row65_col0" class="data row65 col0" >104</td>
      <td id="T_6576c_row65_col1" class="data row65 col1" ></td>
      <td id="T_6576c_row65_col2" class="data row65 col2" ></td>
      <td id="T_6576c_row65_col3" class="data row65 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row66" class="row_heading level0 row66" >2024-01-20</th>
      <td id="T_6576c_row66_col0" class="data row66 col0" >98</td>
      <td id="T_6576c_row66_col1" class="data row66 col1" ></td>
      <td id="T_6576c_row66_col2" class="data row66 col2" ></td>
      <td id="T_6576c_row66_col3" class="data row66 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row67" class="row_heading level0 row67" >2024-01-22</th>
      <td id="T_6576c_row67_col0" class="data row67 col0" >114</td>
      <td id="T_6576c_row67_col1" class="data row67 col1" >105</td>
      <td id="T_6576c_row67_col2" class="data row67 col2" >105</td>
      <td id="T_6576c_row67_col3" class="data row67 col3" >127</td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row68" class="row_heading level0 row68" >2024-01-23</th>
      <td id="T_6576c_row68_col0" class="data row68 col0" >114</td>
      <td id="T_6576c_row68_col1" class="data row68 col1" ></td>
      <td id="T_6576c_row68_col2" class="data row68 col2" ></td>
      <td id="T_6576c_row68_col3" class="data row68 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row69" class="row_heading level0 row69" >2024-01-24</th>
      <td id="T_6576c_row69_col0" class="data row69 col0" >109</td>
      <td id="T_6576c_row69_col1" class="data row69 col1" ></td>
      <td id="T_6576c_row69_col2" class="data row69 col2" ></td>
      <td id="T_6576c_row69_col3" class="data row69 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row70" class="row_heading level0 row70" >2024-01-25</th>
      <td id="T_6576c_row70_col0" class="data row70 col0" >112</td>
      <td id="T_6576c_row70_col1" class="data row70 col1" ></td>
      <td id="T_6576c_row70_col2" class="data row70 col2" ></td>
      <td id="T_6576c_row70_col3" class="data row70 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row71" class="row_heading level0 row71" >2024-01-26</th>
      <td id="T_6576c_row71_col0" class="data row71 col0" >103</td>
      <td id="T_6576c_row71_col1" class="data row71 col1" ></td>
      <td id="T_6576c_row71_col2" class="data row71 col2" ></td>
      <td id="T_6576c_row71_col3" class="data row71 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row72" class="row_heading level0 row72" >2024-01-28</th>
      <td id="T_6576c_row72_col0" class="data row72 col0" >110</td>
      <td id="T_6576c_row72_col1" class="data row72 col1" ></td>
      <td id="T_6576c_row72_col2" class="data row72 col2" ></td>
      <td id="T_6576c_row72_col3" class="data row72 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row73" class="row_heading level0 row73" >2024-01-29</th>
      <td id="T_6576c_row73_col0" class="data row73 col0" >108</td>
      <td id="T_6576c_row73_col1" class="data row73 col1" ></td>
      <td id="T_6576c_row73_col2" class="data row73 col2" ></td>
      <td id="T_6576c_row73_col3" class="data row73 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row74" class="row_heading level0 row74" >2024-01-30</th>
      <td id="T_6576c_row74_col0" class="data row74 col0" >112</td>
      <td id="T_6576c_row74_col1" class="data row74 col1" ></td>
      <td id="T_6576c_row74_col2" class="data row74 col2" ></td>
      <td id="T_6576c_row74_col3" class="data row74 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row75" class="row_heading level0 row75" >2024-01-31</th>
      <td id="T_6576c_row75_col0" class="data row75 col0" >106</td>
      <td id="T_6576c_row75_col1" class="data row75 col1" ></td>
      <td id="T_6576c_row75_col2" class="data row75 col2" ></td>
      <td id="T_6576c_row75_col3" class="data row75 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row76" class="row_heading level0 row76" >2024-02-01</th>
      <td id="T_6576c_row76_col0" class="data row76 col0" >87</td>
      <td id="T_6576c_row76_col1" class="data row76 col1" >100</td>
      <td id="T_6576c_row76_col2" class="data row76 col2" >103</td>
      <td id="T_6576c_row76_col3" class="data row76 col3" >121</td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row77" class="row_heading level0 row77" >2024-02-02</th>
      <td id="T_6576c_row77_col0" class="data row77 col0" >96</td>
      <td id="T_6576c_row77_col1" class="data row77 col1" ></td>
      <td id="T_6576c_row77_col2" class="data row77 col2" ></td>
      <td id="T_6576c_row77_col3" class="data row77 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row78" class="row_heading level0 row78" >2024-02-03</th>
      <td id="T_6576c_row78_col0" class="data row78 col0" >92</td>
      <td id="T_6576c_row78_col1" class="data row78 col1" ></td>
      <td id="T_6576c_row78_col2" class="data row78 col2" ></td>
      <td id="T_6576c_row78_col3" class="data row78 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row79" class="row_heading level0 row79" >2024-02-05</th>
      <td id="T_6576c_row79_col0" class="data row79 col0" >105</td>
      <td id="T_6576c_row79_col1" class="data row79 col1" ></td>
      <td id="T_6576c_row79_col2" class="data row79 col2" ></td>
      <td id="T_6576c_row79_col3" class="data row79 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row80" class="row_heading level0 row80" >2024-02-06</th>
      <td id="T_6576c_row80_col0" class="data row80 col0" >106</td>
      <td id="T_6576c_row80_col1" class="data row80 col1" ></td>
      <td id="T_6576c_row80_col2" class="data row80 col2" ></td>
      <td id="T_6576c_row80_col3" class="data row80 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row81" class="row_heading level0 row81" >2024-02-07</th>
      <td id="T_6576c_row81_col0" class="data row81 col0" >103</td>
      <td id="T_6576c_row81_col1" class="data row81 col1" ></td>
      <td id="T_6576c_row81_col2" class="data row81 col2" ></td>
      <td id="T_6576c_row81_col3" class="data row81 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row82" class="row_heading level0 row82" >2024-02-09</th>
      <td id="T_6576c_row82_col0" class="data row82 col0" >104</td>
      <td id="T_6576c_row82_col1" class="data row82 col1" ></td>
      <td id="T_6576c_row82_col2" class="data row82 col2" ></td>
      <td id="T_6576c_row82_col3" class="data row82 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row83" class="row_heading level0 row83" >2024-02-12</th>
      <td id="T_6576c_row83_col0" class="data row83 col0" >102</td>
      <td id="T_6576c_row83_col1" class="data row83 col1" >101</td>
      <td id="T_6576c_row83_col2" class="data row83 col2" >101</td>
      <td id="T_6576c_row83_col3" class="data row83 col3" >103</td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row84" class="row_heading level0 row84" >2024-02-13</th>
      <td id="T_6576c_row84_col0" class="data row84 col0" >106</td>
      <td id="T_6576c_row84_col1" class="data row84 col1" ></td>
      <td id="T_6576c_row84_col2" class="data row84 col2" ></td>
      <td id="T_6576c_row84_col3" class="data row84 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row85" class="row_heading level0 row85" >2024-02-15</th>
      <td id="T_6576c_row85_col0" class="data row85 col0" >105</td>
      <td id="T_6576c_row85_col1" class="data row85 col1" ></td>
      <td id="T_6576c_row85_col2" class="data row85 col2" ></td>
      <td id="T_6576c_row85_col3" class="data row85 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row86" class="row_heading level0 row86" >2024-02-18</th>
      <td id="T_6576c_row86_col0" class="data row86 col0" >92</td>
      <td id="T_6576c_row86_col1" class="data row86 col1" ></td>
      <td id="T_6576c_row86_col2" class="data row86 col2" ></td>
      <td id="T_6576c_row86_col3" class="data row86 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row87" class="row_heading level0 row87" >2024-02-20</th>
      <td id="T_6576c_row87_col0" class="data row87 col0" >107</td>
      <td id="T_6576c_row87_col1" class="data row87 col1" ></td>
      <td id="T_6576c_row87_col2" class="data row87 col2" ></td>
      <td id="T_6576c_row87_col3" class="data row87 col3" >92</td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row88" class="row_heading level0 row88" >2024-02-21</th>
      <td id="T_6576c_row88_col0" class="data row88 col0" >99</td>
      <td id="T_6576c_row88_col1" class="data row88 col1" ></td>
      <td id="T_6576c_row88_col2" class="data row88 col2" ></td>
      <td id="T_6576c_row88_col3" class="data row88 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row89" class="row_heading level0 row89" >2024-02-22</th>
      <td id="T_6576c_row89_col0" class="data row89 col0" >109</td>
      <td id="T_6576c_row89_col1" class="data row89 col1" ></td>
      <td id="T_6576c_row89_col2" class="data row89 col2" ></td>
      <td id="T_6576c_row89_col3" class="data row89 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row90" class="row_heading level0 row90" >2024-02-23</th>
      <td id="T_6576c_row90_col0" class="data row90 col0" >107</td>
      <td id="T_6576c_row90_col1" class="data row90 col1" ></td>
      <td id="T_6576c_row90_col2" class="data row90 col2" ></td>
      <td id="T_6576c_row90_col3" class="data row90 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row91" class="row_heading level0 row91" >2024-02-25</th>
      <td id="T_6576c_row91_col0" class="data row91 col0" >94</td>
      <td id="T_6576c_row91_col1" class="data row91 col1" ></td>
      <td id="T_6576c_row91_col2" class="data row91 col2" ></td>
      <td id="T_6576c_row91_col3" class="data row91 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row92" class="row_heading level0 row92" >2024-02-26</th>
      <td id="T_6576c_row92_col0" class="data row92 col0" >107</td>
      <td id="T_6576c_row92_col1" class="data row92 col1" ></td>
      <td id="T_6576c_row92_col2" class="data row92 col2" ></td>
      <td id="T_6576c_row92_col3" class="data row92 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row93" class="row_heading level0 row93" >2024-02-27</th>
      <td id="T_6576c_row93_col0" class="data row93 col0" >116</td>
      <td id="T_6576c_row93_col1" class="data row93 col1" >107</td>
      <td id="T_6576c_row93_col2" class="data row93 col2" >83</td>
      <td id="T_6576c_row93_col3" class="data row93 col3" >96</td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row94" class="row_heading level0 row94" >2024-02-28</th>
      <td id="T_6576c_row94_col0" class="data row94 col0" >113</td>
      <td id="T_6576c_row94_col1" class="data row94 col1" ></td>
      <td id="T_6576c_row94_col2" class="data row94 col2" ></td>
      <td id="T_6576c_row94_col3" class="data row94 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row95" class="row_heading level0 row95" >2024-03-04</th>
      <td id="T_6576c_row95_col0" class="data row95 col0" >104</td>
      <td id="T_6576c_row95_col1" class="data row95 col1" ></td>
      <td id="T_6576c_row95_col2" class="data row95 col2" ></td>
      <td id="T_6576c_row95_col3" class="data row95 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row96" class="row_heading level0 row96" >2024-03-06</th>
      <td id="T_6576c_row96_col0" class="data row96 col0" >83</td>
      <td id="T_6576c_row96_col1" class="data row96 col1" ></td>
      <td id="T_6576c_row96_col2" class="data row96 col2" ></td>
      <td id="T_6576c_row96_col3" class="data row96 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row97" class="row_heading level0 row97" >2024-03-07</th>
      <td id="T_6576c_row97_col0" class="data row97 col0" >102</td>
      <td id="T_6576c_row97_col1" class="data row97 col1" ></td>
      <td id="T_6576c_row97_col2" class="data row97 col2" ></td>
      <td id="T_6576c_row97_col3" class="data row97 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row98" class="row_heading level0 row98" >2024-03-11</th>
      <td id="T_6576c_row98_col0" class="data row98 col0" >132</td>
      <td id="T_6576c_row98_col1" class="data row98 col1" ></td>
      <td id="T_6576c_row98_col2" class="data row98 col2" ></td>
      <td id="T_6576c_row98_col3" class="data row98 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row99" class="row_heading level0 row99" >2024-03-12</th>
      <td id="T_6576c_row99_col0" class="data row99 col0" >101</td>
      <td id="T_6576c_row99_col1" class="data row99 col1" ></td>
      <td id="T_6576c_row99_col2" class="data row99 col2" ></td>
      <td id="T_6576c_row99_col3" class="data row99 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row100" class="row_heading level0 row100" >2024-03-13</th>
      <td id="T_6576c_row100_col0" class="data row100 col0" >100</td>
      <td id="T_6576c_row100_col1" class="data row100 col1" ></td>
      <td id="T_6576c_row100_col2" class="data row100 col2" ></td>
      <td id="T_6576c_row100_col3" class="data row100 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row101" class="row_heading level0 row101" >2024-03-15</th>
      <td id="T_6576c_row101_col0" class="data row101 col0" >102</td>
      <td id="T_6576c_row101_col1" class="data row101 col1" ></td>
      <td id="T_6576c_row101_col2" class="data row101 col2" ></td>
      <td id="T_6576c_row101_col3" class="data row101 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row102" class="row_heading level0 row102" >2024-03-17</th>
      <td id="T_6576c_row102_col0" class="data row102 col0" >97</td>
      <td id="T_6576c_row102_col1" class="data row102 col1" ></td>
      <td id="T_6576c_row102_col2" class="data row102 col2" ></td>
      <td id="T_6576c_row102_col3" class="data row102 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row103" class="row_heading level0 row103" >2024-03-18</th>
      <td id="T_6576c_row103_col0" class="data row103 col0" >109</td>
      <td id="T_6576c_row103_col1" class="data row103 col1" >91</td>
      <td id="T_6576c_row103_col2" class="data row103 col2" >92</td>
      <td id="T_6576c_row103_col3" class="data row103 col3" >140</td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row104" class="row_heading level0 row104" >2024-03-19</th>
      <td id="T_6576c_row104_col0" class="data row104 col0" >97</td>
      <td id="T_6576c_row104_col1" class="data row104 col1" ></td>
      <td id="T_6576c_row104_col2" class="data row104 col2" ></td>
      <td id="T_6576c_row104_col3" class="data row104 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row105" class="row_heading level0 row105" >2024-03-20</th>
      <td id="T_6576c_row105_col0" class="data row105 col0" >103</td>
      <td id="T_6576c_row105_col1" class="data row105 col1" ></td>
      <td id="T_6576c_row105_col2" class="data row105 col2" ></td>
      <td id="T_6576c_row105_col3" class="data row105 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row106" class="row_heading level0 row106" >2024-03-21</th>
      <td id="T_6576c_row106_col0" class="data row106 col0" >107</td>
      <td id="T_6576c_row106_col1" class="data row106 col1" ></td>
      <td id="T_6576c_row106_col2" class="data row106 col2" ></td>
      <td id="T_6576c_row106_col3" class="data row106 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row107" class="row_heading level0 row107" >2024-03-23</th>
      <td id="T_6576c_row107_col0" class="data row107 col0" >96</td>
      <td id="T_6576c_row107_col1" class="data row107 col1" ></td>
      <td id="T_6576c_row107_col2" class="data row107 col2" ></td>
      <td id="T_6576c_row107_col3" class="data row107 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row108" class="row_heading level0 row108" >2024-03-24</th>
      <td id="T_6576c_row108_col0" class="data row108 col0" >96</td>
      <td id="T_6576c_row108_col1" class="data row108 col1" ></td>
      <td id="T_6576c_row108_col2" class="data row108 col2" ></td>
      <td id="T_6576c_row108_col3" class="data row108 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row109" class="row_heading level0 row109" >2024-03-25</th>
      <td id="T_6576c_row109_col0" class="data row109 col0" >112</td>
      <td id="T_6576c_row109_col1" class="data row109 col1" ></td>
      <td id="T_6576c_row109_col2" class="data row109 col2" ></td>
      <td id="T_6576c_row109_col3" class="data row109 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row110" class="row_heading level0 row110" >2024-03-26</th>
      <td id="T_6576c_row110_col0" class="data row110 col0" >98</td>
      <td id="T_6576c_row110_col1" class="data row110 col1" >101</td>
      <td id="T_6576c_row110_col2" class="data row110 col2" >100</td>
      <td id="T_6576c_row110_col3" class="data row110 col3" >150</td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row111" class="row_heading level0 row111" >2024-03-28</th>
      <td id="T_6576c_row111_col0" class="data row111 col0" >122</td>
      <td id="T_6576c_row111_col1" class="data row111 col1" ></td>
      <td id="T_6576c_row111_col2" class="data row111 col2" ></td>
      <td id="T_6576c_row111_col3" class="data row111 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row112" class="row_heading level0 row112" >2024-03-29</th>
      <td id="T_6576c_row112_col0" class="data row112 col0" >124</td>
      <td id="T_6576c_row112_col1" class="data row112 col1" ></td>
      <td id="T_6576c_row112_col2" class="data row112 col2" ></td>
      <td id="T_6576c_row112_col3" class="data row112 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row113" class="row_heading level0 row113" >2024-03-30</th>
      <td id="T_6576c_row113_col0" class="data row113 col0" >103</td>
      <td id="T_6576c_row113_col1" class="data row113 col1" ></td>
      <td id="T_6576c_row113_col2" class="data row113 col2" ></td>
      <td id="T_6576c_row113_col3" class="data row113 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row114" class="row_heading level0 row114" >2024-04-01</th>
      <td id="T_6576c_row114_col0" class="data row114 col0" >107</td>
      <td id="T_6576c_row114_col1" class="data row114 col1" ></td>
      <td id="T_6576c_row114_col2" class="data row114 col2" ></td>
      <td id="T_6576c_row114_col3" class="data row114 col3" ></td>
    </tr>
    <tr>
      <th id="T_6576c_level0_row115" class="row_heading level0 row115" >2024-04-02</th>
      <td id="T_6576c_row115_col0" class="data row115 col0" >101</td>
      <td id="T_6576c_row115_col1" class="data row115 col1" ></td>
      <td id="T_6576c_row115_col2" class="data row115 col2" ></td>
      <td id="T_6576c_row115_col3" class="data row115 col3" ></td>
    </tr>
  </tbody>
</table>

</div>