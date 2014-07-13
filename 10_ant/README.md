# Ant

## Antターゲットのインポート

下記コマンドにより、build.xmlに定義されたターゲットをGradleタスクとして実行できるようになる

```
ant.importBuild 'build.xml'
```

## Antタスクの利用

Gradleのスクリプト内で、Antの機能を利用できる

```
task hello << {
    ant.echo("Hello Ant from Gradle!")
}
```

GroovyのAntBuilderを利用している。
[AntBuilder (groovy 2.2.1 API)](http://groovy.codehaus.org/gapi/groovy/util/AntBuilder.html?is-external=true "AntBuilder (groovy 2.2.1 API)")
