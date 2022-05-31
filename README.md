# yazilim-odevi
package com.plcoding.solidprinciplesandroid
import java.io.File
interface FileLogger {
fun printlogs(){
}
fun logError(error:string){
val file =File(pathname:"errors.txt")
file.appendText(
text=error)
}
}
calss custumErrorFilLogger :FileLogger{
override fun logError(error:string){
val file =File(pathname:"my_custum_error_file.txt")
file.appendText(
text=error)
}
}
