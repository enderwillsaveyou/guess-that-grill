# Dataset Documentation

## Overview
This directory contains the quiz dataset for the guess-that-grill application.

## Files

### cars.json
The main quiz data source containing car information with the following structure:

#### Car Record Fields
- **id**: Unique identifier for the car (string)
- - **make**: Car manufacturer/brand (string)
  - - **model**: Car model name (string)
    - - **yearStart**: Start year of production (number)
      - - **yearEnd**: End year of production (number)
        - - **image**: URL path to the car's grill image (string)
          - - **alt**: Alternative text description for the image (string)
           
            - ## Image Storage
           
            - All car images are stored in the `/images` directory at the repository root.
           
            - When images are uploaded to the repository, image URLs in `cars.json` should be updated to use raw GitHub URLs in the format:
            - ```
              https://raw.githubusercontent.com/enderwillsaveyou/guess-that-grill/main/images/[image-filename]
              ```

              ## Adding New Records

              To add a new car to the quiz:
              1. Add an object to the array in `cars.json` with all required fields
              2. 2. Upload the car's grill image to the `/images` folder
                 3. 3. Update the `image` field with the raw GitHub URL to the image
                    4. 
