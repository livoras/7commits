## Post
createTime: Date
editTime: Date
content: String
creator: ObjectId
comments: [ObjectId]
tags: [ObjectId(Tag)]


## Comment
creator: {
    email: String
    name: String
}
content: String
createTime: Date


## Member
name: String
password: String
avatar: String
signature: String
introdution: String
isAdmin: {type: Boolean, default: false}
showMember: {type: Boolean, default: true}


## Tag
name: String
posts: [ObjectId]