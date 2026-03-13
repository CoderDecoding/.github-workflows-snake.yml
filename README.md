name: generate animation

on:
  # run automatically every 24 hours
  schedule:
    - cron: "0 */24 * * *" 
  
  # allows to manually run the job at any time (THIS CREATES THE BUTTON)
  workflow_dispatch:
  
  # run on every push on the main branch
  push:
    branches:
    - main
