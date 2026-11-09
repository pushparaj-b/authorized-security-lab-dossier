# Lab Architecture and Data-Flow Notes

## Intended boundary
The assessment is limited to the two inventory entries supplied for this exercise. LAB-01 is described as localhost. LAB-02 is described as a private host-only VM. External systems, public targets, personal devices, and unlisted assets are excluded.

## Data-flow diagram
See `data_flow_diagram.png`. The diagram is conceptual. It does not assert that LAB-01 and LAB-02 communicate with each other. Confirm the actual network design before documenting any direct connection.

## Suggested safe local practice setup
If the owner/instructor approves a substitute for LAB-01, OWASP Juice Shop can be run locally using Docker with a loopback-only port binding:
```powershell
docker pull bkimminich/juice-shop
docker run -d --name juice-shop -p 127.0.0.1:8080:3000 bkimminich/juice-shop
```
Open `http://127.0.0.1:8080` in the browser. Verify with:
```powershell
docker ps
```
This creates a local training app; it does not prove that the supplied RabTech LAB-01 is present. Do not run the container if the port is already used or if the owner has not approved the substitute.

## LAB-02
Do not create or claim a VM with the supplied IP unless the actual training VM image is provided and the address is verified. If supplied, configure a host-only network and confirm the address with the lab owner. Do not use bridged networking.
