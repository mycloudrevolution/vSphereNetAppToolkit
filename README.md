# vSphereNetAppToolkit PowerShell Module

## About

### Project Owner:

Markus Kraus [@vMarkus_K](https://twitter.com/vMarkus_K)

MY CLOUD-(R)EVOLUTION [mycloudrevolution.com](http://mycloudrevolution.com/)

### Project WebSite:

[mycloudrevolution.com](http://mycloudrevolution.com/)

### Project Repository

[vSphereNetAppToolkit](https://github.com/mycloudrevolution/vSphereNetAppToolkit)

### Project Documentation:

[Read the Docs](http://readthedocs.io/)

### Project Description:

The 'vSphereNetAppToolkit' PowerShell Module ...

## Requirements

 ```PowerShell
Import-Module DataONTAP
Import-Module VMware.VimAutomation.Cis.Core
$NaCreds = Get-Credential -Message "NetApp"
$VcCreds = Get-Credential -Message "vCenter"

Connect-NcController netapp.lab.local -Credential $NaCreds
Connect-VIServer vcenter-01.lab.local -Credential $VcCreds
```

## Functions

## New-VsphereNetappVolume

 ```PowerShell
New-VsphereNetappVolume -VolName vol_vmware_11 -VolSize 1 -vSphereCluster Cluster01 -NetAppAggregate aggr_data -NetAppVserver svm-esxi `
-NetAppInterface svm-nfs_data -NetAppSnapshotPolicy default-1weekly
```

