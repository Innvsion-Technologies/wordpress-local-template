# wordpress-local-template
Template to run wordpress with Docker.



# Create a new directory for your development workspace. The directory should be located somewhere below one of the following paths (depending on your OS):
        - DEFAULT SHARED DIRECTORIES
        - Mac: /Users, /Volumes, /private, & /tmp
        - Windows: C:\Users
        - Linux: /home

# Download or Pull the repositorie. Open a terminal window in your workspace directory and run the following commands:
        - docker-compose up -d
        - docker-compose exec -u 1000 wordpress divi-dev setup

This could take a few minutes (or more) depending on your internet connection speed. 

# Final Step: Access WordPress Dashboard And Install Divi 
        - (https://www.elegantthemes.com/documentation/divi/install-divi/)



# Commands Quick Reference

# You can use the following commands to manage your containers. Be sure to run them from inside your workspace directory:

# Enter Container (get command prompt inside container)
        - docker-compose exec -u 1000 wordpress /bin/bash

# Exit Container (return to your system’s command prompt)
        - exit

# Stop Running Containers
        - docker-compose stop

# Start Stopped Containers
        - docker-compose start

# Remove Containers (WordPress database will be deleted!)
        - docker-compose down

# Start New Containers
        - docker-compose up -d
        - docker-compose exec -u 1000 wordpress divi-dev setup
