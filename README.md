# Flutter Exercise

A Flutter project increase my knowledge and learn how to use it.

## Local Deployment
<ul>
    <ol>
            <p>1. Install Flutter VSCode extension</p>
            <p>2. Clone the repository</p>
            <p>3. Run the application with 'Flutter run' in the CLI</p>
    </ol>
</ul>

```bash
Git clone https://github.com/mhykol2k/flutter_exercise.git
```

## Example

![This is an image](https://i.imgur.com/hGK0ekw.png)

## Code Examples

### How the user increments, decrements and resets the counter.

```dart
class _MyHomePageState extends State<MyHomePage> {
  int _counter = 0;

  void _incrementCounter() {
    setState(() {
      _counter++;
    });
  }

  void _decrementCounter() {
    setState(() {
      _counter--;
    });
  }

  void _resetCounter() {
    setState(() {
      _counter = 0;
    });
  }
```

### Body of the application

```dart
      body: Center(
        child: Padding(
          padding: const EdgeInsets.all(8.0),
          child: Column(
            mainAxisAlignment: MainAxisAlignment.center,
            crossAxisAlignment: CrossAxisAlignment.center,
            children: <Widget>[
              const Text(
                'The count is at...',
                textAlign: TextAlign.center,
              ),
              Text(
                '$_counter',
                style: Theme.of(context).textTheme.headline4,
              ),
              FloatingActionButton(
                onPressed: _incrementCounter,
                tooltip: 'Increment Counter',
                child: const Icon(Icons.add),
              ),
              FloatingActionButton(
                onPressed: _decrementCounter,
                tooltip: 'Decrement Counter',
                child: const Icon(Icons.remove),
              ),
              FloatingActionButton(
                onPressed: _resetCounter,
                tooltip: 'Reset Counter',
                child: const Icon(Icons.select_all_sharp),
              ),
```

## Getting Started

For help getting started with Flutter development, view the
[online documentation](https://docs.flutter.dev/), which offers tutorials,
samples, guidance on mobile development, and a full API reference.
