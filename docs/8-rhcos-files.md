# RHCOS files

Download the RHCOS ISO, BIOS and UEFI image files:

```bash
OCPMAJOR="4.4"
OCPVERSION="4.4.3"
RCHOSVERSION="4.4.3"
BASE_URL="https://mirror.openshift.com/pub/openshift-v4/dependencies/rhcos/4.4/${OCPVERSION}"
HOME_DIR=""
for asset in 'installer.iso' 'metal.x86_64.raw.gz'; do
  curl -J -L ${BASE_URL}/rhcos-${RHCOSVERSION}-x86_64-${asset} -o ${HOME_DIR}/rhcos-${RHCOSVERSION}-x86_64-${asset}
done
```

[<< Previous: Ignition files](7-ignition-files.md) | [README](../README.md) | [Next: Modify ISOs >>](9-modify-isos.md)
