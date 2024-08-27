#Belajar Gradle

#build.gradle yang dibuat ditambahkan kode berikut :
Task greetingTask() {
    doLast {
        String nama = project.hasProperty('nama') ? project.property('nama') : 'Gradle User'
        println "Hello, $nama! Welcome to Gradle World!"
    }
}

#Untuk menjalankan gradle bisa dilakukan diterminal dengan memasukan code berikut :
./gradlew greetingTask -Pnama=Kevin
