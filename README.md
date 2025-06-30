# Campground-Locator

'A Full Stack Application - Build for the Learning Purpose'


The following illustration is for my own understanding and 
the future reference.

            * ==== In The Second Commit ===== *
Added : models/campground.js
i.e. added the basic model and check it.
Note :the result of "db.campgrounds.find()"
 yelp-camp> db.campgrounds.find()
[
  {
    _id: ObjectId('68622c8c6a27b6a282e861e3'),
    description: 'cheap camping !',
    __v: 0
  },
  {
    _id: ObjectId('6862307aa2e590f256ddcc2c'),
    title: 'My Backyard',
    description: 'cheap camping !',
    __v: 0
  }
]
In models/campground.js :
module.exports = mongoose.model('Campground', CampgroundSchema);
 'campgrounds' is Actual MongoDB collection name (auto-lowered & pluralized by Mongoose) 

Issue : Every time we visited / refreshed the browser
a now 'id' will be saved in database. This can be fixed by 
proper seeding.
