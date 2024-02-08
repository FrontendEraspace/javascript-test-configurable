# Product Configurable / Javascript Test Searching

we have a data below, the data is an array of object that contains color and storage.
it is not fixed data, maybe in the future we have another choice or type.

```javascript
var pilihan = [
  { color: "merah", storage: 64 },
  { color: "biru", storage: 128 },
  { color: "hijau", storage: 256 },
]
```

## User Story

As a user, I want to be able find user choice form the array "pilihan" so that i can find the index of the choice.

```javascript
var pilihanPengguna1 = { color: "biru", storage: 128 }
var pilihanPengguna2 = { storage: 128, color: "biru" } // Properti terbalik
var pilihanPengguna3 = { color: "merah" } // Properti kurang

function bandingkan() {
  // your code here ..
}

var hasilPencarian1 = bandingkan(pilihan, pilihanPengguna1)
var hasilPencarian2 = bandingkan(pilihan, pilihanPengguna2)
var hasilPencarian3 = bandingkan(pilihan, pilihanPengguna3)

console.log("Indeks pilihan 1 yang cocok:", hasilPencarian1) // Output: 1
console.log("Indeks pilihan 2 yang cocok:", hasilPencarian2) // Output: 1
console.log("Indeks pilihan 3 yang cocok:", hasilPencarian3) // Output: -1
```

## Expected Result

Indeks pilihan 1 yang cocok: 1 <br />
Indeks pilihan 2 yang cocok: 1 <br />
Indeks pilihan 3 yang cocok: -1
