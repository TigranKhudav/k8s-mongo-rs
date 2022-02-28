# k8s mongo replica set

1. apply sts 
2. ` rs.initiate() `
3. ` rs.initiate( {
...    _id : "rs1",
...    members: [
...       { _id: 0, host: "10.10.10.60:27017" },
...       { _id: 1, host: "10.10.10.86:27017" },
...       { _id: 2, host: "10.10.10.87:27017" },
...    ]
... }) `
