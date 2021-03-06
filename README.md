# InfluxDb Jenkins Plugin

By Eficode Ltd (https://github.com/eficode).

This plugin allows you to send the build metrics to InfluxDb servers to be used for analysis and radiators. 
Tested with InfluxDb 0.12 and 0.13.

# Instructions

Build with `mvn package`. Creates a `target` directory, with a `.hpi` file in it. Upload the `.hpi` file to Jenkins.

## Jenkins configuration
The url-parameter needs the whole url in order to work including the `http://` (e.g `http://127.0.0.1:8086`)

# Supported Metrics
- project_name
- build_number
- build_time
- build_status_message
- project_build_health
- tests_failed
- tests_skipped
- tests_total
- cobertura_package_coverage_rate
- cobertura_class_coverage_rate
- cobertura_line_coverage_rate
- cobertura_branch_coverage_rate
- cobertura_number_of_packages
- cobertura_number_of_sourcefiles
- cobertura_number_of_classes
- Robot Framework plugin metrics

# Special Thanks
Plugin originally developed by Jouni Rajala (https://twitter.com/rajalajouni) and updated to use InfluxDb 0.9+ with the help of http://christoph-burmeister.eu/?p=2906.
