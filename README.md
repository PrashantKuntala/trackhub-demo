# trackhub-demo

This repo is a demo to host a UCSC trackhub on GitHub to visualize bigWigs and bigBeds.

### Steps to connect trackhub-demo to UCSC genome browser

- Go to [UCSC genome browser](https://genome.ucsc.edu/) and goto `My Data > Track Hubs`
- Now select the `My Hubs` tab on the page.
- Copy and paste the below url into the `URL` field and click on `Add Hub`
  - `https://raw.githubusercontent.com/prashantkuntala/trackhub-demo/main/hub.txt`

This should load the trackhub. UCSC genome browser will redirect after selecting the organism specified in the `hub.txt` file. Click on `Go` and you should see your trackhub loaded as a section in the track selector interface.

> If you wish to host all your bigwigs on a different server, you can do so by deleting the `sacCer3/data/` folder and updating `bigDataUrl`, in the `subtracks.txt` file, to contain the absolute filepath for each sample's bigwig on the external server.
