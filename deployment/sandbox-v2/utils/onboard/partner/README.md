# Partner onboarding

## Onboarding steps
1. Add policy group
1. Add policy 
1. Add partner
1. Create and upload partner certificates
1. Map partner to policy
1. Add MISP

## Script
1. Make sure you run `./preinstall.sh`  for Python dependencies.
1. Point to your sandbox in `config.py`:
    ```
    server='<your sandbox doman>'
    ```
1. Populate the CSVs in `csv` folder.  
1. Update/add any policies in `policies` folder.  The schema for policies are given here:
    * [Auth policy schema](https://github.com/mosip/mosip-config/blob/1.1.3/sandbox/auth-policy-schema.json)
    * [Data share schema](https://github.com/mosip/mosip-config/blob/1.1.3/sandbox/data-share-policy-schema.json)
1.  Run the script as below:
    ```
    $ ./partner.py <action>
    For actions see help. The actions here map to steps above:  
    $ ./partner.py --help
    ```