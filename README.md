# csharpcode

## Date Picker

### STEP 01 
```html
                <div class="form-group row">
                    <div class="col-4">
                        Select Date
                    </div>
                    <div class="col-8">
                        <input asp-for="EventDate" type="text" class="form-control datepicker"/>
                        <span asp-validation-for="EventDate" class="text-danger"></span>
                    </div>
                </div>
```

### STEP 02

```js
<script>
        // Data Picker Initialization
        $(document).ready(function () {
            $('.datepicker').datepicker({
                dateFormat: "dd/mm/yy",
                showStatus: true,
                showWeeks: true,
                currentText: 'Now',
                autoSize: true,
                gotoCurrent: true,
                showAnim: 'blind',
                highlightWeek: true
            });
        });

    </script>
```
