# Data Engineer Challenge

## Requirements
- Spark 2.4.5
- Python libs: pweave, Bokeh and boto3. 

If you run this on Amazon EMR, you should install pweave and Bokeh at cluster bootstrap time.

## Usage
```
spark-submit src/process.py <nyc_json_file> <vendor_csv_file> <payment_csv_file> <output_bucket> <output_path_to_JSON_and_HTML>
```

If you run this script on EMR, just add the spark submit as a EMR Step. The script also need to be uploaded on S3.

## Report analysis
[Download Report](report/report.html)

## TODO
- AWS Cloudformation to bootstrap EMR Cluster
- Logs
- Unit tests