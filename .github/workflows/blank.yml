
class MainActivity : ComponentActivity() {
    override fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState)
        enableEdgeToEdge()
        setContent {
            MyVedioApplicationTheme {
                Column() {
                    var timeOfday =

                        arrayOf("morning", "early morning", "sunrise", "afternoon", "evening")

                }
                Column() {
                    Text("timeOfday[1]")
                    var suggestion = arrayOf(
                        "sends a good morning",
                        "sends a good early morning",
                        "sends a good sunrise",
                        "sends a good afternoon",
                        "sends a good evening"

                    )
                    var text by remember { mutableStateOf("") }
                    var results by remember { mutableStateOf("") }

                    OutlinedTextField(
                        value = text,
                        onValueChange = { text = it },
                        label = { Text("Enter time of the day") }
                    )
                    Button(
                        onClick = {
                            results = when (text) {
                                "morning" -> "send a good morning text"
                                "early morning" -> "send a good early morning text"
                                "sunrise" -> "send a good sunrise text"
                                "afternoon" -> "send a good afternoon text"
                                "sunset" ->"send a good sunset text"
                                else -> "Invalid input"

                            }
                        }
                    ) {
                        Text("suggestion")
                    }
                    Button(
                        onClick = {
                            text = ""
                            results = ""
                        }
                    ) {
                        Text("reset")
                    }
                    Text(results)

                }
            }
        }
    }
}




