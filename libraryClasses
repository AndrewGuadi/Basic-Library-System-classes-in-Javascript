class libraryItem {
  constructor(title){
    this._title = title;
    this._isCheckedOut = false;
    this._ratings = []
  }
  get title(){
    if (this._title){
      return this._title;
    }
    else{
      console.log('There is no title available')
    }
  }
  get isCheckedOut(){
    return isCheckedOut;
  }
  get ratings(){
    if (this._ratings){
      return this._ratings;
    }
  }
  getAverageRating(){
    if (this._ratings){
      var totalRate = 0;
      this._ratings.forEach(rating => totalRate += rating);
      const avgRate = totalRate / this._ratings.length;
      return avgRate;
    }
  }
  toggleCheckoutStatus(){
    this._isCheckedOut = !this._isCheckedOut;
  }
  addRating(newRating){
    if (typeof newRating === 'number'){
      this._ratings.push(newRating);
    }
  }
}

class book extends libraryItem{
  constructor(title, author, pages){
    super(title);
    this._author = author;
    this._pages = pages;
  }
  get author(){
    if (this._author){
      return this._author;
    }
    else{
      console.log('This is no Author logged')
    }
  }
  get pages(){
    if (this._pages){
      return this._pages;
    }
    else{
      console.log('No number of pages found');
    }
  }
}

class cd extends libraryItem{
  constructor(title, artist, songs){
    super(title);
    this._artist = artist;
    this._songs = [songs];
  }
  get artist(){
    if (this._artist){
      return this._artist;
    }
    else{
      console.log('There is no Artist listed')
    }
  }
  get songs(){
    if (this._songs){
      return this._songs;
    }
    else{
      console.log('There is no Track list')
    }
  }
}

class movie extends libraryItem{
  constructor(title, director, runTime){
    super(title);
    this._director = director;
    this._runTime = ((typeof runTime === 'number') ? runTime : 0)
  }
  set runTime(movieTime){
    if (typeof movieTime === ' number' && movieTime > 0){
      this._runTime = runTime;
    }
    else{
      console.log('Please choose an positive integer for movie run time')
    }
  }
  get director(){
    if (this._director){
      return this._director;
    }
    else{
      console.log('There was no director listed')
    }
  }
  get runTime(){
    if (this._runTime){
      return this._runTime;
    }
  }
}
