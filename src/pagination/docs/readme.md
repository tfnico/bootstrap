A lightweight pagination directive that is focused on ... providing pagination & will take care of visualising a pagination bar and enable / disable buttons correctly!

### Pagination Settings ###

Settings can be provided as attributes in the `<pagination>` or globally configured through the `paginationConfig`.

 * `num-pages` <i class="icon-eye-open"></i>
 	:
 	Number of total pages.

 * `current-page` <i class="icon-eye-open"></i>
 	:
 	Current page number.

 * `max-size` <i class="icon-eye-open"></i>
 	_(Defaults: null)_ :
 	Limit number for pagination size.

 * `rotate`
 	_(Defaults: true)_ :
 	Whether to keep current page in the middle of the visible ones.

 * `on-select-page (page)`
 	_(Default: null)_ :
 	An optional expression called when a page is selected having the page number as argument.

 * `direction-links`
 	_(Default: true)_ :
 	Whether to display Previous / Next buttons.

 * `previous-text`
 	_(Default: 'Previous')_ :
 	Text for Previous button.

 * `next-text`
 	_(Default: 'Next')_ :
 	Text for Next button.

 * `boundary-links`
 	_(Default: false)_ :
 	Whether to display First / Last buttons.

 * `first-text`
 	_(Default: 'First')_ :
 	Text for First button.

 * `last-text`
 	_(Default: 'Last')_ :
 	Text for Last button.

### Pager Settings ###

Settings can be provided as attributes in the `<pager>` or globally configured through the `pagerConfig`.  
For `num-pages`,  `current-page` and `on-select-page (page)` see pagination settings. Other settings are:

 * `align`
 	_(Default: true)_ :
 	Whether to align each link to the sides.

 * `previous-text`
 	_(Default: '« Previous')_ :
 	Text for Previous button.

 * `next-text`
 	_(Default: 'Next »')_ :
 	Text for Next button.

### Styling ###


You may also want to add some custom styles to the pagination elements:

    .pagination {
      cursor:pointer;

      text-align: center;
      -webkit-user-select: none; /* Chrome/Safari */
      -moz-user-select: none; /* Firefox */
      -ms-user-select: none; /* IE10+ */

      /* Rules below not implemented in browsers yet */
      -o-user-select: none;
      user-select: none;
    }

The above example will:

* Switch the curser to pointer-mode while hovering over page numbers
* Disable text selection
