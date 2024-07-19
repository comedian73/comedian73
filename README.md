Олдырев Николай '\n'
Возраст: <a id="age"></a>















<script>
function getAge() {
    let teg = document.getElementById('age');
    var dateString = "1992-10-07";
    var today = new Date();
    var birthDate = new Date(dateString);
    var age = today.getFullYear() - birthDate.getFullYear();
    var m = today.getMonth() - birthDate.getMonth();
    if (m < 0 || (m === 0 && today.getDate() < birthDate.getDate())) {
        age--;
    }
    return teg.append(age);
}
</script>
