# k8s mongo replica set

1. apply sts 
2. ` rs.initiate() `
3. ` rs.initiate( {
...    _id : "rs1",
...    members: [
...       { _id: 0, host: "mongo-0.default.svc.cluster.local:27017" },
...       { _id: 1, host: "mongo-w1.default.svc.cluster.local:27017" },
...       { _id: 2, host: "mongo-w2.default.svc.cluster.local:27017" },
...    ]
... }) `
