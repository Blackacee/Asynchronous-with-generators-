# Asynchronous-with-generators-

function someAsyncResult() {
 return Promise.resolve('newValue')
}
q.spawn(function * () {
 var result = yield someAsyncResult()
 console.log(result) // 'newValue'
})
