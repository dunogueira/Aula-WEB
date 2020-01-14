# Aula-WEB

let num = document.querySelector('input#fnum')
let lista = document.qerySelector('select#flista')
let res = document.querySelector('div#res')
let valores = []

function isNumero(n){
    if(Number(n) >= 1 && Number(n) <= 100){
        return true 
    } else {
        return false
    }
}

function inLista(n, l) {
    if(l.indexOf(Number(n)) != -1) {
        return true
    } else {
        return false
    }
}

function adicionar() {
   if(isNumero(num.value) && !inLista(num.value, valores)) {
       window.alert('ok, inserido')
   } else {
       window.alert('valor invalido ou ja add na lista')
   }
}c
