
# Users Collection

# 1- mongosh
run command 
-mongosh

# 2- show dbs
-show dbs
admin     41 kB
config  36.9 kB
local   73.7 kB
masai    274 kB

# 3- use database assignment
use the database called assignment
- use assignment
switched to db assignment

# 4- using collection called users in assignment database
- db.users.insert({"first_name":"Eward","last_name":"Brownett","email":"ebrownett0@cafepress.com","gender":"Male","ip_address":"19.208.43.193","age":35})

{
  acknowledged: true,
  insertedIds: { '0': ObjectId("61ffb574ea60414c44d94f54") }
}

# 5- show collections
- show collections
users

# 6- using insertMany
- db.users.insertMany([{ "first_name": "Temp", "last_name": "Heggman", "email": "theggman1@tumblr.com", "gender": "Agender", "ip_address": "100.101.204.179", "age": 48 }, { "first_name": "Lester", "last_name": "Bestiman", "email": "lbestiman2@imdb.com", "gender": "Male", "ip_address": "144.18.222.112", "age": 43 }, { "first_name": "Alleyn", "last_name": "Blanket", "email": "ablanket3@webeden.co.uk", "gender": "Female", "ip_address": "89.131.29.48", "age": 48 }, { "first_name": "Murdoch", "last_name": "Rowat", "email": "mrowat4@tripadvisor.com", "gender": "Female", "ip_address": "88.228.201.126", "age": 40 }, { "first_name": "Darn", "last_name": "Artois", "email": "dartois5@noaa.gov", "gender": "Female", "ip_address": "59.212.154.157", "age": 22 }, { "first_name": "Jerald", "last_name": "McGuggy", "email": "jmcguggy6@redcross.org", "gender": "Bigender", "ip_address": "11.36.215.171", "age": 21 }, { "first_name": "Flin", "last_name": "MacGlory", "email": "fmacglory7@fda.gov", "gender": "Male", "ip_address": "241.178.68.81", "age": 47 }, { "first_name": "Klement", "last_name": "Beevor", "email": "kbeevor8@hubpages.com", "gender": "Male", "ip_address": "41.35.138.144", "age": 37 }, { "first_name": "Elihu", "last_name": "Sermin", "email": "esermin9@whitehouse.gov", "gender": "Genderfluid", "ip_address": "0.55.179.90", "age": 24 }])
{  acknowledged: true,  insertedIds: {    '0': ObjectId("61ffb6deea60414c44d94f55"),    '1': ObjectId("61ffb6deea60414c44d94f56"),    '2': ObjectId("61ffb6deea60414c44d94f57"),
    '3': ObjectId("61ffb6deea60414c44d94f58"),
    '4': ObjectId("61ffb6deea60414c44d94f59"),
    '5': ObjectId("61ffb6deea60414c44d94f5a"),
    '6': ObjectId("61ffb6deea60414c44d94f5b"),
    '7': ObjectId("61ffb6deea60414c44d94f5c"),
    '8': ObjectId("61ffb6deea60414c44d94f5d")
  }
}

# 7- using find 
- db.users.find()
[
  {
    _id: ObjectId("61ffb574ea60414c44d94f54"),
    first_name: 'Eward',
    last_name: 'Brownett',
    email: 'ebrownett0@cafepress.com',
    gender: 'Male',
    ip_address: '19.208.43.193',
    age: 35
  },
  {
    _id: ObjectId("61ffb6deea60414c44d94f55"),
    first_name: 'Temp',
    last_name: 'Heggman',
    email: 'theggman1@tumblr.com',
    gender: 'Agender',
    ip_address: '100.101.204.179',
    age: 48
  },
  {
    _id: ObjectId("61ffb6deea60414c44d94f56"),
    first_name: 'Lester',
    last_name: 'Bestiman',
    email: 'lbestiman2@imdb.com',
    gender: 'Male',
    ip_address: '144.18.222.112',
    age: 43
  },
  {
    _id: ObjectId("61ffb6deea60414c44d94f57"),
    first_name: 'Alleyn',
    last_name: 'Blanket',
    email: 'ablanket3@webeden.co.uk',
    gender: 'Female',
    ip_address: '89.131.29.48',
    age: 48
  },
  {
    _id: ObjectId("61ffb6deea60414c44d94f58"),
    first_name: 'Murdoch',
    last_name: 'Rowat',
    email: 'mrowat4@tripadvisor.com',
    gender: 'Female',
    ip_address: '88.228.201.126',
    age: 40
  },
  {
    _id: ObjectId("61ffb6deea60414c44d94f59"),
    first_name: 'Darn',
    last_name: 'Artois',
    email: 'dartois5@noaa.gov',
    gender: 'Female',
    ip_address: '59.212.154.157',
    age: 22
  },
  {
    _id: ObjectId("61ffb6deea60414c44d94f5a"),
    first_name: 'Jerald',
    last_name: 'McGuggy',
    email: 'jmcguggy6@redcross.org',
    gender: 'Bigender',
    ip_address: '11.36.215.171',
    age: 21
  },
  {
    _id: ObjectId("61ffb6deea60414c44d94f5b"),
    first_name: 'Flin',
    last_name: 'MacGlory',
    email: 'fmacglory7@fda.gov',
    gender: 'Male',
    ip_address: '241.178.68.81',
    age: 47
  },
  {
    _id: ObjectId("61ffb6deea60414c44d94f5c"),
    first_name: 'Klement',
    last_name: 'Beevor',
    email: 'kbeevor8@hubpages.com',
    gender: 'Male',
    ip_address: '41.35.138.144',
    age: 37
  },
  {
    _id: ObjectId("61ffb6deea60414c44d94f5d"),
    first_name: 'Elihu',
    last_name: 'Sermin',
    email: 'esermin9@whitehouse.gov',
    gender: 'Genderfluid',
    ip_address: '0.55.179.90',
    age: 24
  }
]

# 8- db.users-findOne()
- db.users.findOne({_id: ObjectId("61ffb6deea60414c44d94f5b")})
{
  _id: ObjectId("61ffb6deea60414c44d94f5b"),
  first_name: 'Flin',
  last_name: 'MacGlory',
  email: 'fmacglory7@fda.gov',
  gender: 'Male',
  ip_address: '241.178.68.81',
  age: 47
}

# 9- Update at least 3 documents using update and updateMany

# updateOne
- db.users.updateOne({_id: ObjectId("61ffb574ea60414c44d94f54")},{$set: {gender: "female"}})        
{
  acknowledged: true,
  insertedId: null,
  matchedCount: 1,
  modifiedCount: 1,
  upsertedCount: 0
}

- db.users.findOne({_id: ObjectId("61ffb574ea60414c44d94f54")})
{
  _id: ObjectId("61ffb574ea60414c44d94f54"),
  first_name: 'Eward',
  last_name: 'Brownett',
  email: 'ebrownett0@cafepress.com',
  gender: 'female',
  ip_address: '19.208.43.193',
  age: 35
}

# 10- updateMany()
- db.users.updateMany({gender: "Male"},{$set: {gender: "female"}})    
{
  acknowledged: true,
  insertedId: null,
  matchedCount: 3,
  modifiedCount: 3,
  upsertedCount: 0
}

- db.users.find()
[
  {
    _id: ObjectId("61ffb574ea60414c44d94f54"),
    first_name: 'Eward',
    last_name: 'Brownett',
    email: 'ebrownett0@cafepress.com',
    gender: 'female',
    ip_address: '19.208.43.193',
    age: 35
  },
  {
    _id: ObjectId("61ffb6deea60414c44d94f55"),
    first_name: 'Temp',
    last_name: 'Heggman',
    email: 'theggman1@tumblr.com',
    gender: 'Agender',
    ip_address: '100.101.204.179',
    age: 48
  },
  {
    _id: ObjectId("61ffb6deea60414c44d94f56"),
    first_name: 'Lester',
    last_name: 'Bestiman',
    email: 'lbestiman2@imdb.com',
    gender: 'female',
    ip_address: '144.18.222.112',
    age: 43
  },
  {
    _id: ObjectId("61ffb6deea60414c44d94f57"),
    first_name: 'Alleyn',
    last_name: 'Blanket',
    email: 'ablanket3@webeden.co.uk',
    gender: 'Female',
    ip_address: '89.131.29.48',
    age: 48
  },
  {
    _id: ObjectId("61ffb6deea60414c44d94f58"),
    first_name: 'Murdoch',
    last_name: 'Rowat',
    email: 'mrowat4@tripadvisor.com',
    gender: 'Female',
    ip_address: '88.228.201.126',
    age: 40
  },
  {
    _id: ObjectId("61ffb6deea60414c44d94f59"),
    first_name: 'Darn',
    last_name: 'Artois',
    email: 'dartois5@noaa.gov',
    gender: 'Female',
    ip_address: '59.212.154.157',
    age: 22
  },
  {
    _id: ObjectId("61ffb6deea60414c44d94f5a"),
    first_name: 'Jerald',
    last_name: 'McGuggy',
    email: 'jmcguggy6@redcross.org',
    gender: 'Bigender',
    ip_address: '11.36.215.171',
    age: 21
  },
  {
    _id: ObjectId("61ffb6deea60414c44d94f5b"),
    first_name: 'Flin',
    last_name: 'MacGlory',
    email: 'fmacglory7@fda.gov',
    gender: 'female',
    ip_address: '241.178.68.81',
    age: 47
  },
  {
    _id: ObjectId("61ffb6deea60414c44d94f5c"),
    first_name: 'Klement',
    last_name: 'Beevor',
    email: 'kbeevor8@hubpages.com',
    gender: 'female',
    ip_address: '41.35.138.144',
    age: 37
  },
  {
    _id: ObjectId("61ffb6deea60414c44d94f5d"),
    first_name: 'Elihu',
    last_name: 'Sermin',
    email: 'esermin9@whitehouse.gov',
    gender: 'Genderfluid',
    ip_address: '0.55.179.90',
    age: 24
  }
]

# 11- Delete documents using remove, remove that will remove just 1 document, deleteOne, deleteMany

# deleteOne
- db.users.deleteOne({_id: ObjectId("61ffb574ea60414c44d94f54")})
{ acknowledged: true, deletedCount: 1 }

- db.users.find()
[
  {
    _id: ObjectId("61ffb6deea60414c44d94f55"),
    first_name: 'Temp',
    last_name: 'Heggman',
    email: 'theggman1@tumblr.com',
    gender: 'Agender',
    ip_address: '100.101.204.179',
    age: 48
  },
  {
    _id: ObjectId("61ffb6deea60414c44d94f56"),
    first_name: 'Lester',
    last_name: 'Bestiman',
    email: 'lbestiman2@imdb.com',
    gender: 'female',
    ip_address: '144.18.222.112',
    age: 43
  },
  {
    _id: ObjectId("61ffb6deea60414c44d94f57"),
    first_name: 'Alleyn',
    last_name: 'Blanket',
    email: 'ablanket3@webeden.co.uk',
    gender: 'Female',
    ip_address: '89.131.29.48',
    age: 48
  },
  {
    _id: ObjectId("61ffb6deea60414c44d94f58"),
    first_name: 'Murdoch',
    last_name: 'Rowat',
    email: 'mrowat4@tripadvisor.com',
    gender: 'Female',
    ip_address: '88.228.201.126',
    age: 40
  },
  {
  {
    _id: ObjectId("61ffb6deea60414c44d94f5b"),
    first_name: 'Flin',
    last_name: 'MacGlory',
    email: 'fmacglory7@fda.gov',
    gender: 'female',
    ip_address: '241.178.68.81',
    age: 47
  },
  {
    _id: ObjectId("61ffb6deea60414c44d94f5c"),
    first_name: 'Klement',
    last_name: 'Beevor',
    email: 'kbeevor8@hubpages.com',
    gender: 'female',
    ip_address: '41.35.138.144',
    age: 37
  },
  {
    _id: ObjectId("61ffb6deea60414c44d94f5d"),
    first_name: 'Elihu',
    last_name: 'Sermin',
    email: 'esermin9@whitehouse.gov',
    gender: 'Genderfluid',
    ip_address: '0.55.179.90',
    age: 24
  }
]

# deleteMany({})
- db.users.deleteMany({gender: "female"})
{ acknowledged: true, deletedCount: 3 }

- db.users.find()
[
  {
    _id: ObjectId("61ffb6deea60414c44d94f55"),
    first_name: 'Temp',
    last_name: 'Heggman',
    email: 'theggman1@tumblr.com',
    gender: 'Agender',
    ip_address: '100.101.204.179',
    age: 48
  },
  {
    _id: ObjectId("61ffb6deea60414c44d94f57"),
    first_name: 'Alleyn',
    last_name: 'Blanket',
    email: 'ablanket3@webeden.co.uk',
    gender: 'Female',
    ip_address: '89.131.29.48',
    age: 48
  },
  {
    _id: ObjectId("61ffb6deea60414c44d94f58"),
    first_name: 'Murdoch',
    last_name: 'Rowat',
    email: 'mrowat4@tripadvisor.com',
    gender: 'Female',
    ip_address: '88.228.201.126',
    age: 40
  },
  {
    _id: ObjectId("61ffb6deea60414c44d94f59"),
    first_name: 'Darn',
    last_name: 'Artois',
    email: 'dartois5@noaa.gov',
    gender: 'Female',
    ip_address: '59.212.154.157',
    age: 22
  },
  {
    _id: ObjectId("61ffb6deea60414c44d94f5a"),
    first_name: 'Jerald',
    last_name: 'McGuggy',
    email: 'jmcguggy6@redcross.org',
    gender: 'Bigender',
    ip_address: '11.36.215.171',
    age: 21
  },
  {
    _id: ObjectId("61ffb6deea60414c44d94f5d"),
    first_name: 'Elihu',
    last_name: 'Sermin',
    email: 'esermin9@whitehouse.gov',
    gender: 'Genderfluid',
    ip_address: '0.55.179.90',
    age: 24
  }
]

# 12- delete the database
- db.dropDatabase()
{ ok: 1, dropped: 'assignment' }

# 13- show collections
assignment> show collections

assignment>

- show dbs
admin     41 kB
config   111 kB
local   73.7 kB
masai    274 kB
