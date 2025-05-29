# MongoDB_assignment

```javascript
use admin
switched to db admin
use practise
switched to db practise
db.todo_table.insertOne({task : "Play",
status:"Not done"})
{
  acknowledged: true,
  insertedId: ObjectId('6837f3730339644fb49baadc')
}
db.todo_table.insertMany([
  {task : 'dance',status: "Not done"},
  {task : 'sing',status :" Not done"},
  {task : 'Study',status : "Done"}
])
{
  acknowledged: true,
  insertedIds: {
    '0': ObjectId('6837f3840339644fb49baadd'),
    '1': ObjectId('6837f3840339644fb49baade'),
    '2': ObjectId('6837f3840339644fb49baadf')
  }
}
db.todo_table.updateMany({status : "Done"},
                         {$set : {status:true}})
{
  acknowledged: true,
  insertedId: null,
  matchedCount: 1,
  modifiedCount: 1,
  upsertedCount: 0
}
db.todo_table.find()
{
  _id: ObjectId('6837f306bd56136471088441'),
  task: 'Play',
  status: 'Not done'
}
{
  _id: ObjectId('6837f312bd56136471088442'),
  task: 'dance',
  status: 'Not done'
}
{
  _id: ObjectId('6837f312bd56136471088443'),
  task: 'sing',
  status: ' Not done'
}
{
  _id: ObjectId('6837f312bd56136471088444'),
  task: 'Study',
  status: true
}
{
  _id: ObjectId('6837f3730339644fb49baadc'),
  task: 'Play',
  status: 'Not done'
}
{
  _id: ObjectId('6837f3840339644fb49baadd'),
  task: 'dance',
  status: 'Not done'
}
{
  _id: ObjectId('6837f3840339644fb49baade'),
  task: 'sing',
  status: ' Not done'
}
{
  _id: ObjectId('6837f3840339644fb49baadf'),
  task: 'Study',
  status: true
}
db.todo_table.updateMany({status : "Not Done"},
                         {$set : {status:false}})
{
  acknowledged: true,
  insertedId: null,
  matchedCount: 0,
  modifiedCount: 0,
  upsertedCount: 0
}
db.todo_table.find()
{
  _id: ObjectId('6837f306bd56136471088441'),
  task: 'Play',
  status: 'Not done'
}
{
  _id: ObjectId('6837f312bd56136471088442'),
  task: 'dance',
  status: 'Not done'
}
{
  _id: ObjectId('6837f312bd56136471088443'),
  task: 'sing',
  status: ' Not done'
}
{
  _id: ObjectId('6837f312bd56136471088444'),
  task: 'Study',
  status: true
}
{
  _id: ObjectId('6837f3730339644fb49baadc'),
  task: 'Play',
  status: 'Not done'
}
{
  _id: ObjectId('6837f3840339644fb49baadd'),
  task: 'dance',
  status: 'Not done'
}
{
  _id: ObjectId('6837f3840339644fb49baade'),
  task: 'sing',
  status: ' Not done'
}
{
  _id: ObjectId('6837f3840339644fb49baadf'),
  task: 'Study',
  status: true
}
db.todo_table.updateMany({status : 'Not Done'},
                         {$set : {status:false}})
{
  acknowledged: true,
  insertedId: null,
  matchedCount: 0,
  modifiedCount: 0,
  upsertedCount: 0
}
db.todo_table.find()
{
  _id: ObjectId('6837f306bd56136471088441'),
  task: 'Play',
  status: 'Not done'
}
{
  _id: ObjectId('6837f312bd56136471088442'),
  task: 'dance',
  status: 'Not done'
}
{
  _id: ObjectId('6837f312bd56136471088443'),
  task: 'sing',
  status: ' Not done'
}
{
  _id: ObjectId('6837f312bd56136471088444'),
  task: 'Study',
  status: true
}
{
  _id: ObjectId('6837f3730339644fb49baadc'),
  task: 'Play',
  status: 'Not done'
}
{
  _id: ObjectId('6837f3840339644fb49baadd'),
  task: 'dance',
  status: 'Not done'
}
{
  _id: ObjectId('6837f3840339644fb49baade'),
  task: 'sing',
  status: ' Not done'
}
{
  _id: ObjectId('6837f3840339644fb49baadf'),
  task: 'Study',
  status: true
}
db.todo_table.updateMany({status : 'Not done'},
                         {$set : {status:false}})
{
  acknowledged: true,
  insertedId: null,
  matchedCount: 4,
  modifiedCount: 4,
  upsertedCount: 0
}
db.todo_table.find()
{
  _id: ObjectId('6837f306bd56136471088441'),
  task: 'Play',
  status: false
}
{
  _id: ObjectId('6837f312bd56136471088442'),
  task: 'dance',
  status: false
}
{
  _id: ObjectId('6837f312bd56136471088443'),
  task: 'sing',
  status: ' Not done'
}
{
  _id: ObjectId('6837f312bd56136471088444'),
  task: 'Study',
  status: true
}
{
  _id: ObjectId('6837f3730339644fb49baadc'),
  task: 'Play',
  status: false
}
{
  _id: ObjectId('6837f3840339644fb49baadd'),
  task: 'dance',
  status: false
}
{
  _id: ObjectId('6837f3840339644fb49baade'),
  task: 'sing',
  status: ' Not done'
}
{
  _id: ObjectId('6837f3840339644fb49baadf'),
  task: 'Study',
  status: true
}
db.todo_table.updateMany({status : ' Not done'},
                         {$set : {status:false}})
{
  acknowledged: true,
  insertedId: null,
  matchedCount: 2,
  modifiedCount: 2,
  upsertedCount: 0
}
db.todo_table.find()
{
  _id: ObjectId('6837f306bd56136471088441'),
  task: 'Play',
  status: false
}
{
  _id: ObjectId('6837f312bd56136471088442'),
  task: 'dance',
  status: false
}
{
  _id: ObjectId('6837f312bd56136471088443'),
  task: 'sing',
  status: false
}
{
  _id: ObjectId('6837f312bd56136471088444'),
  task: 'Study',
  status: true
}
{
  _id: ObjectId('6837f3730339644fb49baadc'),
  task: 'Play',
  status: false
}
{
  _id: ObjectId('6837f3840339644fb49baadd'),
  task: 'dance',
  status: false
}
{
  _id: ObjectId('6837f3840339644fb49baade'),
  task: 'sing',
  status: false
}
{
  _id: ObjectId('6837f3840339644fb49baadf'),
  task: 'Study',
  status: true
}
db.todo_table.insertMany([
  {task : 'shopping',status: true},
  {task : 'go for a walk',status :false},
  {task : 'chill with friends',status : true}
])
{
  acknowledged: true,
  insertedIds: {
    '0': ObjectId('6837f4ff0339644fb49baae0'),
    '1': ObjectId('6837f4ff0339644fb49baae1'),
    '2': ObjectId('6837f4ff0339644fb49baae2')
  }
}
db.todo_table.find()
{
  _id: ObjectId('6837f306bd56136471088441'),
  task: 'Play',
  status: false
}
{
  _id: ObjectId('6837f312bd56136471088442'),
  task: 'dance',
  status: false
}
{
  _id: ObjectId('6837f312bd56136471088443'),
  task: 'sing',
  status: false
}
{
  _id: ObjectId('6837f312bd56136471088444'),
  task: 'Study',
  status: true
}
{
  _id: ObjectId('6837f3730339644fb49baadc'),
  task: 'Play',
  status: false
}
{
  _id: ObjectId('6837f3840339644fb49baadd'),
  task: 'dance',
  status: false
}
{
  _id: ObjectId('6837f3840339644fb49baade'),
  task: 'sing',
  status: false
}
{
  _id: ObjectId('6837f3840339644fb49baadf'),
  task: 'Study',
  status: true
}
{
  _id: ObjectId('6837f4ff0339644fb49baae0'),
  task: 'shopping',
  status: true
}
{
  _id: ObjectId('6837f4ff0339644fb49baae1'),
  task: 'go for a walk',
  status: false
}
{
  _id: ObjectId('6837f4ff0339644fb49baae2'),
  task: 'chill with friends',
  status: true
}
db.todo_table.insertMany([
  {task : 'Eat',status: false},
  {task : 'Sleep',status :true},
  {task : 'Talk to parents',status : true}
])
{
  acknowledged: true,
  insertedIds: {
    '0': ObjectId('6837f51b0339644fb49baae3'),
    '1': ObjectId('6837f51b0339644fb49baae4'),
    '2': ObjectId('6837f51b0339644fb49baae5')
  }
}
db.todo_table.find()
{
  _id: ObjectId('6837f306bd56136471088441'),
  task: 'Play',
  status: false
}
{
  _id: ObjectId('6837f312bd56136471088442'),
  task: 'dance',
  status: false
}
{
  _id: ObjectId('6837f312bd56136471088443'),
  task: 'sing',
  status: false
}
{
  _id: ObjectId('6837f312bd56136471088444'),
  task: 'Study',
  status: true
}
{
  _id: ObjectId('6837f3730339644fb49baadc'),
  task: 'Play',
  status: false
}
{
  _id: ObjectId('6837f3840339644fb49baadd'),
  task: 'dance',
  status: false
}
{
  _id: ObjectId('6837f3840339644fb49baade'),
  task: 'sing',
  status: false
}
{
  _id: ObjectId('6837f3840339644fb49baadf'),
  task: 'Study',
  status: true
}
{
  _id: ObjectId('6837f4ff0339644fb49baae0'),
  task: 'shopping',
  status: true
}
{
  _id: ObjectId('6837f4ff0339644fb49baae1'),
  task: 'go for a walk',
  status: false
}
{
  _id: ObjectId('6837f4ff0339644fb49baae2'),
  task: 'chill with friends',
  status: true
}
{
  _id: ObjectId('6837f51b0339644fb49baae3'),
  task: 'Eat',
  status: false
}
{
  _id: ObjectId('6837f51b0339644fb49baae4'),
  task: 'Sleep',
  status: true
}
{
  _id: ObjectId('6837f51b0339644fb49baae5'),
  task: 'Talk to parents',
  status: true
}
db.todo_table.updateMany(
  { status: { $exists: false } },
  { $set: { status: false } }
);
{
  acknowledged: true,
  insertedId: null,
  matchedCount: 0,
  modifiedCount: 0,
  upsertedCount: 0
}
db.todo_table.insertOne([
  {task : 'Clockout'}
])
{
  acknowledged: true,
  insertedId: ObjectId('6837f5430339644fb49baae6')
}
db.todo_table.find()
{
  _id: ObjectId('6837f306bd56136471088441'),
  task: 'Play',
  status: false
}
{
  _id: ObjectId('6837f312bd56136471088442'),
  task: 'dance',
  status: false
}
{
  _id: ObjectId('6837f312bd56136471088443'),
  task: 'sing',
  status: false
}
{
  _id: ObjectId('6837f312bd56136471088444'),
  task: 'Study',
  status: true
}
{
  _id: ObjectId('6837f3730339644fb49baadc'),
  task: 'Play',
  status: false
}
{
  _id: ObjectId('6837f3840339644fb49baadd'),
  task: 'dance',
  status: false
}
{
  _id: ObjectId('6837f3840339644fb49baade'),
  task: 'sing',
  status: false
}
{
  _id: ObjectId('6837f3840339644fb49baadf'),
  task: 'Study',
  status: true
}
{
  _id: ObjectId('6837f4ff0339644fb49baae0'),
  task: 'shopping',
  status: true
}
{
  _id: ObjectId('6837f4ff0339644fb49baae1'),
  task: 'go for a walk',
  status: false
}
{
  _id: ObjectId('6837f4ff0339644fb49baae2'),
  task: 'chill with friends',
  status: true
}
{
  _id: ObjectId('6837f51b0339644fb49baae3'),
  task: 'Eat',
  status: false
}
{
  _id: ObjectId('6837f51b0339644fb49baae4'),
  task: 'Sleep',
  status: true
}
{
  _id: ObjectId('6837f51b0339644fb49baae5'),
  task: 'Talk to parents',
  status: true
}
{
  '0': {
    task: 'Clockout'
  },
  _id: ObjectId('6837f5430339644fb49baae6')
}
db.todo_table.updateOne(
  {_id : ObjectId('6836e8fe31485535101b3925')},
  {$set : {status : true}}
)
{
  acknowledged: true,
  insertedId: null,
  matchedCount: 0,
  modifiedCount: 0,
  upsertedCount: 0
}
db.todo_table.updateMany(
  { status: { $exists: true } },
  { $push: { createdAt: new Date() } }
);
{
  acknowledged: true,
  insertedId: null,
  matchedCount: 14,
  modifiedCount: 14,
  upsertedCount: 0
}
db.runCommand({
  collMod: "todo_table",
  validator: {
    $jsonSchema: {
      bsonType: "object",
      properties: {
        priority: {
          enum: ["low", "medium", "high"]
        }
      }}}})
{ ok: 1 }
db.todo_table.updateMany(
  { name: { $exists: true } },
  { $set: { priority : "medium" } }
);
{
  acknowledged: true,
  insertedId: null,
  matchedCount: 0,
  modifiedCount: 0,
  upsertedCount: 0
}
db.todo_table.updateMany(
   { name: { $exists: true } },
  { $set: { priority : "medium" } }
);
{
  acknowledged: true,
  insertedId: null,
  matchedCount: 0,
  modifiedCount: 0,
  upsertedCount: 0
}
db.todo_table.find()
{
  _id: ObjectId('6836e42631485535101b391b'),
  task: 'Play',
  status: false,
  updateAt: [
    2025-05-28T10:51:15.761Z
  ],
  createdAt: [
    2025-05-28T10:51:24.829Z
  ]
}
SyntaxError: Missing semicolon. (4:6)

[0m [90m 2 |[39m {
 [90m 3 |[39m   _id[33m:[39m [33mObjectId[39m([32m'6836e42631485535101b391b'[39m)[33m,[39m
[31m[1m>[22m[39m[90m 4 |[39m   task[33m:[39m [32m'Play'[39m[33m,[39m
 [90m   |[39m       [31m[1m^[22m[39m
 [90m 5 |[39m   status[33m:[39m [36mfalse[39m[33m,[39m
 [90m 6 |[39m   updateAt[33m:[39m [
 [90m 7 |[39m     [35m2025[39m[33m-[39m[35m05[39m[33m-[39m[35m28[39m[33mT10[39m[33m:[39m[35m51[39m[33m:[39m[35m15.761[39m[33mZ[39m[0m
db.todo_table.find()
{
  _id: ObjectId('6837f306bd56136471088441'),
  task: 'Play',
  status: false,
  createdAt: [
    2025-05-29T05:54:00.806Z
  ]
}
{
  _id: ObjectId('6837f312bd56136471088442'),
  task: 'dance',
  status: false,
  createdAt: [
    2025-05-29T05:54:00.806Z
  ]
}
{
  _id: ObjectId('6837f312bd56136471088443'),
  task: 'sing',
  status: false,
  createdAt: [
    2025-05-29T05:54:00.806Z
  ]
}
{
  _id: ObjectId('6837f312bd56136471088444'),
  task: 'Study',
  status: true,
  createdAt: [
    2025-05-29T05:54:00.806Z
  ]
}
{
  _id: ObjectId('6837f3730339644fb49baadc'),
  task: 'Play',
  status: false,
  createdAt: [
    2025-05-29T05:54:00.806Z
  ]
}
{
  _id: ObjectId('6837f3840339644fb49baadd'),
  task: 'dance',
  status: false,
  createdAt: [
    2025-05-29T05:54:00.806Z
  ]
}
{
  _id: ObjectId('6837f3840339644fb49baade'),
  task: 'sing',
  status: false,
  createdAt: [
    2025-05-29T05:54:00.806Z
  ]
}
{
  _id: ObjectId('6837f3840339644fb49baadf'),
  task: 'Study',
  status: true,
  createdAt: [
    2025-05-29T05:54:00.806Z
  ]
}
{
  _id: ObjectId('6837f4ff0339644fb49baae0'),
  task: 'shopping',
  status: true,
  createdAt: [
    2025-05-29T05:54:00.806Z
  ]
}
{
  _id: ObjectId('6837f4ff0339644fb49baae1'),
  task: 'go for a walk',
  status: false,
  createdAt: [
    2025-05-29T05:54:00.806Z
  ]
}
{
  _id: ObjectId('6837f4ff0339644fb49baae2'),
  task: 'chill with friends',
  status: true,
  createdAt: [
    2025-05-29T05:54:00.806Z
  ]
}
{
  _id: ObjectId('6837f51b0339644fb49baae3'),
  task: 'Eat',
  status: false,
  createdAt: [
    2025-05-29T05:54:00.806Z
  ]
}
{
  _id: ObjectId('6837f51b0339644fb49baae4'),
  task: 'Sleep',
  status: true,
  createdAt: [
    2025-05-29T05:54:00.806Z
  ]
}
{
  _id: ObjectId('6837f51b0339644fb49baae5'),
  task: 'Talk to parents',
  status: true,
  createdAt: [
    2025-05-29T05:54:00.806Z
  ]
}
{
  '0': {
    task: 'Clockout'
  },
  _id: ObjectId('6837f5430339644fb49baae6')
}
db.todo_table.updateMany(
  { priority: { $exists: false } },  
  { $set: { priority: "low" } }       
);
{
  acknowledged: true,
  insertedId: null,
  matchedCount: 15,
  modifiedCount: 15,
  upsertedCount: 0
}
db.todo_table.updateMany(
  { task : 'Clock in'},  
  { $set: { priority: "low" } }       
);
{
  acknowledged: true,
  insertedId: null,
  matchedCount: 0,
  modifiedCount: 0,
  upsertedCount: 0
}
db.todo_table.insertOne(
  { task : 'Clock in',status : 'false'}      
);
{
  acknowledged: true,
  insertedId: ObjectId('6837f71a0339644fb49baae7')
}
db.todo_table.updateOne(
  { task : 'Clock in'},  
  { $set: { status: true ,updatedAt : new Date()} }       
);
{
  acknowledged: true,
  insertedId: null,
  matchedCount: 1,
  modifiedCount: 1,
  upsertedCount: 0
}
db.todo_table.find()
{
  _id: ObjectId('6837f306bd56136471088441'),
  task: 'Play',
  status: false,
  createdAt: [
    2025-05-29T05:54:00.806Z
  ],
  priority: 'low'
}
{
  _id: ObjectId('6837f312bd56136471088442'),
  task: 'dance',
  status: false,
  createdAt: [
    2025-05-29T05:54:00.806Z
  ],
  priority: 'low'
}
{
  _id: ObjectId('6837f312bd56136471088443'),
  task: 'sing',
  status: false,
  createdAt: [
    2025-05-29T05:54:00.806Z
  ],
  priority: 'low'
}
{
  _id: ObjectId('6837f312bd56136471088444'),
  task: 'Study',
  status: true,
  createdAt: [
    2025-05-29T05:54:00.806Z
  ],
  priority: 'low'
}
{
  _id: ObjectId('6837f3730339644fb49baadc'),
  task: 'Play',
  status: false,
  createdAt: [
    2025-05-29T05:54:00.806Z
  ],
  priority: 'low'
}
{
  _id: ObjectId('6837f3840339644fb49baadd'),
  task: 'dance',
  status: false,
  createdAt: [
    2025-05-29T05:54:00.806Z
  ],
  priority: 'low'
}
{
  _id: ObjectId('6837f3840339644fb49baade'),
  task: 'sing',
  status: false,
  createdAt: [
    2025-05-29T05:54:00.806Z
  ],
  priority: 'low'
}
{
  _id: ObjectId('6837f3840339644fb49baadf'),
  task: 'Study',
  status: true,
  createdAt: [
    2025-05-29T05:54:00.806Z
  ],
  priority: 'low'
}
{
  _id: ObjectId('6837f4ff0339644fb49baae0'),
  task: 'shopping',
  status: true,
  createdAt: [
    2025-05-29T05:54:00.806Z
  ],
  priority: 'low'
}
{
  _id: ObjectId('6837f4ff0339644fb49baae1'),
  task: 'go for a walk',
  status: false,
  createdAt: [
    2025-05-29T05:54:00.806Z
  ],
  priority: 'low'
}
{
  _id: ObjectId('6837f4ff0339644fb49baae2'),
  task: 'chill with friends',
  status: true,
  createdAt: [
    2025-05-29T05:54:00.806Z
  ],
  priority: 'low'
}
{
  _id: ObjectId('6837f51b0339644fb49baae3'),
  task: 'Eat',
  status: false,
  createdAt: [
    2025-05-29T05:54:00.806Z
  ],
  priority: 'low'
}
{
  _id: ObjectId('6837f51b0339644fb49baae4'),
  task: 'Sleep',
  status: true,
  createdAt: [
    2025-05-29T05:54:00.806Z
  ],
  priority: 'low'
}
{
  _id: ObjectId('6837f51b0339644fb49baae5'),
  task: 'Talk to parents',
  status: true,
  createdAt: [
    2025-05-29T05:54:00.806Z
  ],
  priority: 'low'
}
{
  '0': {
    task: 'Clockout'
  },
  _id: ObjectId('6837f5430339644fb49baae6'),
  priority: 'low'
}
{
  _id: ObjectId('6837f71a0339644fb49baae7'),
  task: 'Clock in',
  status: true,
  updatedAt: 2025-05-29T05:56:52.483Z
}
db.todo_table.countDocuments()
16
db.todo_table.find().sort()
{
  _id: ObjectId('6837f306bd56136471088441'),
  task: 'Play',
  status: false,
  createdAt: [
    2025-05-29T05:54:00.806Z
  ],
  priority: 'low'
}
{
  _id: ObjectId('6837f312bd56136471088442'),
  task: 'dance',
  status: false,
  createdAt: [
    2025-05-29T05:54:00.806Z
  ],
  priority: 'low'
}
{
  _id: ObjectId('6837f312bd56136471088443'),
  task: 'sing',
  status: false,
  createdAt: [
    2025-05-29T05:54:00.806Z
  ],
  priority: 'low'
}
{
  _id: ObjectId('6837f312bd56136471088444'),
  task: 'Study',
  status: true,
  createdAt: [
    2025-05-29T05:54:00.806Z
  ],
  priority: 'low'
}
{
  _id: ObjectId('6837f3730339644fb49baadc'),
  task: 'Play',
  status: false,
  createdAt: [
    2025-05-29T05:54:00.806Z
  ],
  priority: 'low'
}
{
  _id: ObjectId('6837f3840339644fb49baadd'),
  task: 'dance',
  status: false,
  createdAt: [
    2025-05-29T05:54:00.806Z
  ],
  priority: 'low'
}
{
  _id: ObjectId('6837f3840339644fb49baade'),
  task: 'sing',
  status: false,
  createdAt: [
    2025-05-29T05:54:00.806Z
  ],
  priority: 'low'
}
{
  _id: ObjectId('6837f3840339644fb49baadf'),
  task: 'Study',
  status: true,
  createdAt: [
    2025-05-29T05:54:00.806Z
  ],
  priority: 'low'
}
{
  _id: ObjectId('6837f4ff0339644fb49baae0'),
  task: 'shopping',
  status: true,
  createdAt: [
    2025-05-29T05:54:00.806Z
  ],
  priority: 'low'
}
{
  _id: ObjectId('6837f4ff0339644fb49baae1'),
  task: 'go for a walk',
  status: false,
  createdAt: [
    2025-05-29T05:54:00.806Z
  ],
  priority: 'low'
}
{
  _id: ObjectId('6837f4ff0339644fb49baae2'),
  task: 'chill with friends',
  status: true,
  createdAt: [
    2025-05-29T05:54:00.806Z
  ],
  priority: 'low'
}
{
  _id: ObjectId('6837f51b0339644fb49baae3'),
  task: 'Eat',
  status: false,
  createdAt: [
    2025-05-29T05:54:00.806Z
  ],
  priority: 'low'
}
{
  _id: ObjectId('6837f51b0339644fb49baae4'),
  task: 'Sleep',
  status: true,
  createdAt: [
    2025-05-29T05:54:00.806Z
  ],
  priority: 'low'
}
{
  _id: ObjectId('6837f51b0339644fb49baae5'),
  task: 'Talk to parents',
  status: true,
  createdAt: [
    2025-05-29T05:54:00.806Z
  ],
  priority: 'low'
}
{
  '0': {
    task: 'Clockout'
  },
  _id: ObjectId('6837f5430339644fb49baae6'),
  priority: 'low'
}
{
  _id: ObjectId('6837f71a0339644fb49baae7'),
  task: 'Clock in',
  status: true,
  updatedAt: 2025-05-29T05:56:52.483Z
}
db.todo_table.updateMany(
  { task: { $exists: true } },
  { $set: { dueDate : new Date() } }
);
{
  acknowledged: true,
  insertedId: null,
  matchedCount: 15,
  modifiedCount: 15,
  upsertedCount: 0
}
db.todo_table.find(
  {dueDate : {$eq : new Date()}}
);
db.todo_table.find(
  {dueDate : {$eq : new Date(28)}}
);


```
