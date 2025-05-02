// Mengambil elemen-elemen HTML
const input1 = document.getElementById('input1');
const input2 = document.getElementById('input2');
const result = document.getElementById('result');

document.getElementById('addButton').addEventListener('click', function() {
    result.textContent = parseFloat(input1.value) + parseFloat(input2.value);
});

document.getElementById('subtractButton').addEventListener('click', function() {
    result.textContent = parseFloat(input1.value) - parseFloat(input2.value);
});

document.getElementById('multiplyButton').addEventListener('click', function() {
    result.textContent = parseFloat(input1.value) * parseFloat(input2.value);
});

document.getElementById('divideButton').addEventListener('click', function() {
    if (parseFloat(input2.value) === 0) {
        result.textContent = 'Tidak dapat dibagi dengan 0';
    } else {
        result.textContent = parseFloat(input1.value) / parseFloat(input2.value);
    }
});
