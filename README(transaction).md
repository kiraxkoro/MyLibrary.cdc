import Library from 0x01
transaction(_title: String, _author: String){

prepare(acct:AuthAccount){

}

execute{
  Library.addBook(_title:_title,_author:_author)
             
}


}
