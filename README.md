# rancheraddon
This includes compmemnts to be integrated into manged kuberntes cluster
These compoments will be installed during setup of new kubernetes cluster
it will be intagred in Ranchers rke addons_include

Each component needs to be integred in rke file 
# check also: https://rancher.com/docs/rke/v0.1.x/en/config-options/add-ons/user-defined-add-ons/#referencing-yaml-files-for-add-ons

addons_include:
    - https://raw.githubusercontent.com/rook/rook/master/cluster/examples/kubernetes/ceph/operator.yaml
    - https://raw.githubusercontent.com/rook/rook/master/cluster/examples/kubernetes/ceph/cluster.yaml
    - /opt/manifests/example.yaml
    - ./nginx.yaml