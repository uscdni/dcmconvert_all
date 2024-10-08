# Scripts to batch run gears on Flywheel

To run these scripts, you must have the [Flywheel python api](https://flywheel-io.gitlab.io/product/backend/sdk/tags/19.1.0/python/getting_started.html#installation) installed. 
You can install the flywheel api with the following command: 

`pip install flywheel-sdk`

## classify_all.py
Runs the scitran classifier gear on all the acquisitions within a session. This gear can be a pre-requisite for alter gears like the mriqc gear. 

Usage: 

**`classify_all.py <full path to session> <api key file>`**

- full path to session: this should be in the format of group/subject/session
    e.g. jtkaplan/SUB01/Kaplan^Moviescans

- api key file: this is a text file that contains your api key. Make one on Flywheel by clicking on your profile.

## dcmconvert_all.py
Runs the dcm2niix gear on all the acquisitions within a session. 

Usage: 

**`dcmconvert_all.py <full path to session> <api key file>`**

- full path to session: this should be in the format of group/subject/session
    e.g. jtkaplan/SUB01/Kaplan^Moviescans

- api key file: this is a text file that contains your api key. Make one on Flywheel by clicking on your profile.

