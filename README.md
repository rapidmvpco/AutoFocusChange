# AutoFocusChange

Here is the code snippet for advancing to the next widget in your Flutterflow app:

``Future changeFocus(
  BuildContext context,
  String inputValue,
) async {
  final FocusScopeNode focus = FocusScope.of(context);

  if (inputValue.length == 1) focus.nextFocus();
}``


Here is the code snippet for reversing to the previous widget based on input length being 0:

``Future reverseFocus(
  BuildContext context,
  String inputValue,
) async {
  final FocusScopeNode focus = FocusScope.of(context);

  if (inputValue.isEmpty) focus.previousFocus();
}``
