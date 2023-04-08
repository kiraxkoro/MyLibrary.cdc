pub contract Library {
    pub var books: [Book]

    pub struct Book {
        pub let title: String
        pub let author: String

        init(_title: String, _author: String) {
            self.title = _title
            self.author = _author
        }
    }

    init() {
        self.books = []
    }

    pub fun addBook(_title: String, _author: String) {
        let newBook = Book(_title: _title, _author: _author)
        self.books.append(newBook)
    }


}
