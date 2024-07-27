✅マイクラをマルチプレイに対応して、敵を倒して点数加算するコードです。


✅「Class com.sun.tools.javac.tree.JCTree$JCImport does not have member field 'com.sun.tools.javac.tree.JCTree qualid'」のエラー


✅原因→LombokとJavaコンパイラ（javac）の互換性に問題


✅解決方法→build.gradleの中身のコードをLombokの最新バージョンに変える
dependencies {
    implementation "org.spigotmc:spigot-api:1.20.6-R0.1-SNAPSHOT"

    implementation 'org.projectlombok:lombok:1.18.34'　←　最新バージョンにする
    annotationProcessor 'org.projectlombok:lombok:1.18.34'　←　最新バージョンにする

    testImplementation 'org.projectlombok:lombok:1.18.34'　←　最新バージョンにする
    testAnnotationProcessor 'org.projectlombok:lombok:1.18.34'　←　最新バージョンにする
}


✅Lombok最新バージョンのサイト(以下のURL)
https://projectlombok.org/changelog
